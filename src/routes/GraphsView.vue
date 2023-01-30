<script>

import Graph from '../components/GraphComponent.vue'

export default {
    name: 'GraphView',
    components: {
        Graph,
    },
}

</script>

<template>
    <div class="graphCell">
        <Graph title="Bar Graph"><div>A bar graph</div></Graph>
        <Graph title="Line Graph"><div>A line graph</div></Graph>
    </div>
    <div class="graphCell">
        <Graph title="Pie Chart"><div> pie chart</div></Graph>
        <Graph title="Heat Map"><div>A heat chart</div></Graph>
    </div>

</template>

<style>
    .graphCell
    {
        display: flex;
        flex-direction: row;
        justify-content: space-evenly;
        margin: 20px;
    }
</style>
