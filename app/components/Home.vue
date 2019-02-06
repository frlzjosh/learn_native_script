<template>
    <Page class="page">
        <ActionBar class="action-bar">
            <Label class="action-bar-title" text="Home"></Label>
        </ActionBar>

        <GridLayout>
            <Label class="title__bar" :text="title" row="1" col="1"></Label>
        </GridLayout>
    </Page>
</template>

<script>
    export default {
        data(){
            return{
                title: "Josh's Native App",
                sup: 'lol',
            }
        },
        computed: {
            message() {
                return "Blank {N}-Vue app";
            }
        }
    };
</script>

<style scoped lang="scss">
    // Start custom common variables
    @import '../app-variables';
    // End custom common variables

    // Custom styles
    .fa {
        color: $accent-dark;
    }

    .info {
        font-size: 20;
    }
</style>
