<template>
    <b-table
        hover
        selectable
        head-variant="dark"
        :fields="fields"
        :items="items"
        select-mode="multi"
        ref="selectableTable"
        @row-selected="onRowSelected"
        show-empty
    >
        <template #empty="scope">
            <h4>{{ scope.emptyText }}</h4>
        </template>
    </b-table>
</template>

<script>
export default {
    name: "ProposalsTable",
    props: ["items", "variant"],
    data() {
        return {
            fields: [
                {key: "numero",                         label: "Nº",                                sortable: true},
                {key: "designacao",                     label: "Designação/Tema" },
                {key: "modulos",                        label: "N.º módulos",                       sortable: true},
                {key: "areas",                          label: "Área temática",                     sortable: true},
                {key: "orientador",                     label: "Orientador",                        sortable: true},
                {key: "coorientadores",                 label: "Coorientadores",                    sortable: true},
                {key: "departamentos_coorientadores",   label: "Departamentos Coorientadores" },
                {key: "Orientador(es) externos",        label: "Orientador(es) externos",           sortable: true},
                {key: "parcerias",                      label: "Parcerias",                         sortable: true},
                {key: "contactos",                      label: "Contacto(s)",                       sortable: true}
            ],
            selected: []
        }
    },
    methods: {
        onRowSelected(items) {
            this.selected = items
        },
        addToInterestingProposals(){
            this.$store.commit("addToInterestingProposals", this.selected)
            this.clearSelected()
        },
        removeFromInterestingProposals(){
            this.$store.commit("removeFromInterestingProposals", this.selected)
            this.clearSelected()
        },
        removeFromNotInterestingProposals(){
            this.$store.commit("removeFromNotInterestingProposals", this.selected)
            this.clearSelected()
        },
        addToNotInterestingProposals(){
            this.$store.commit("addToNotInterestingProposals", this.selected)
            this.clearSelected()
        },
        clearSelected() {
            this.$refs.selectableTable.clearSelected()
        },
    }
}
</script>

<style>
table * {
    font-family: "Segoe UI" !important;
    font-size: small !important;
}

table {
    border-collapse: separate !important;
    border-spacing: 0 !important;
}

th {
    border: 0px !important;
    vertical-align: middle !important;
}

tr td:first-child{
    border-left: 1px solid #dee2e6 !important;
}

tr td:last-child{
    border-right: 1px solid #dee2e6 !important;
}

table tr:first-child td {
    border-top: 0px !important;
}

table tr:last-child td {
    border-bottom: 1px solid #dee2e6 !important;
}

/* top-left border-radius */
table tr:first-child th:first-child {
    border-top-left-radius: 10px !important;
}

/* top-right border-radius */
table tr:first-child th:last-child {
    border-top-right-radius: 10px !important;
}

/* bottom-left border-radius */
table tr:last-child td:first-child {
    border-bottom-left-radius: 10px !important;
}

/* bottom-right border-radius */
table tr:last-child td:last-child {
    border-bottom-right-radius: 10px !important;
}

.table.b-table > tbody > .table-active {
    background-color: rgba(0, 0, 0, 0.2) !important;
}
</style>
