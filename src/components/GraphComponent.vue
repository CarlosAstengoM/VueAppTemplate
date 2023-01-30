<script>

    export default {
        name: `Graph`,
        vm: 
        {
            vmText: "This will later have a graph",
        },
        props: 
        {
            title: String,
        },
        methods: 
        {
            doIt()
            {
                alert("did something")
            }
        }
    }

</script>

<template>
    <div class="borderedSquare">
        <h1 class="title">{{ title }}</h1>
        <h3> <slot> A Graph </slot> </h3>
        <button @click="doIt">Do Something</button>
    </div>
</template>

<style scoped>
    .borderedSquare
    {
        height: 300px;
        width: 500px;
        border-color: black;
        border-style: solid;
        background-color: #334d6b;
    }

    .title
    {
        color: black;
        padding-bottom: 15px;
    }


</style>