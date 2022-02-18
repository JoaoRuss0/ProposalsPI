<template>
    <div id="floating_options">
        <b-button
            class="mb-2"
            variant="success"
            @click.prevent="addToInterestingProposals"
        >Interested 🤤</b-button>

        <b-button
            class="mb-2"
            variant="primary"
            @click.prevent="removeFromInterestingProposals"
        >Not anymore 😢</b-button>

        <b-button
            class="mb-2"
            variant="warning"
            @click.prevent="removeFromNotInterestingProposals"
        >Hmmm 🤔</b-button>

        <b-button
            variant="danger"
            @click.prevent="addToNotInterestingProposals"
        >Ew 🤢</b-button>
    </div>
</template>

<script>
export default {
    name: "FloatingOptions",
    methods: {
        addToInterestingProposals() {
            this.$emit('addToInterestingProposals')
        },
        removeFromInterestingProposals() {
            this.$emit('removeFromInterestingProposals')
        },
        removeFromNotInterestingProposals() {
            this.$emit('removeFromNotInterestingProposals')
        },
        addToNotInterestingProposals() {
            this.$emit('addToNotInterestingProposals')
        }
    }
}
</script>

<style>
#floating_options {
    position: fixed;
    z-index: 1;
    right: 1%;
    top: 20%;
    padding: 20px;
    border: 1px solid black;
    border-radius: 10px;
    background-color: #919194;
    display: flex;
    flex-direction: column;
}
</style>
