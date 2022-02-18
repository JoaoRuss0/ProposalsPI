<template>
    <div class="p-5">
        <b-container fluid>
            <FloatingOptions
                @addToInterestingProposals="addToInterestingProposals"
                @removeFromInterestingProposals="removeFromInterestingProposals"
                @removeFromNotInterestingProposals="removeFromNotInterestingProposals"
                @addToNotInterestingProposals="addToNotInterestingProposals"
            ></FloatingOptions>

            <h3 class="mb-2 text-success">Top picks:</h3>
            <ProposalsTable :items="interesting" ref="interestingProposalsTable"></ProposalsTable>

            <h3 class="mt-4 text-secondary">Choices ..... choices:</h3>
            <ProposalsTable :items="items" ref="allProposalsTable"></ProposalsTable>

            <h3 class="mt-4 text-danger">Worst picks:</h3>
            <ProposalsTable :items="notInteresting" ref="notInterestingProposalsTable"></ProposalsTable>
        </b-container>
    </div>
</template>

<script>
import FloatingOptions from "../components/FloatingOptions";
import ProposalsTable from "../components/ProposalsTable";
export default {
    components: {ProposalsTable, FloatingOptions},
    data() {
        return {
            items: [],
            interesting: [],
            notInteresting: []
        }
    },
    created() {
        this.items = this.$store.getters.getProposals
        this.interesting = this.$store.getters.getInteresting
        this.notInteresting = this.$store.getters.getNotInteresting
    },
    methods: {
        addToInterestingProposals() {
            this.$refs.allProposalsTable.addToInterestingProposals()
        },
        removeFromInterestingProposals() {
            this.$refs.interestingProposalsTable.removeFromInterestingProposals()
        },
        removeFromNotInterestingProposals() {
            this.$refs.notInterestingProposalsTable.removeFromNotInterestingProposals()
        },
        addToNotInterestingProposals() {
            this.$refs.allProposalsTable.addToNotInterestingProposals()
        }
    }
}
</script>

<style>

</style>
