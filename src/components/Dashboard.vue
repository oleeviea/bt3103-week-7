<template>
  <div>
    <BarChart></BarChart>
    <LineChart></LineChart>
  </div>
  
</template>

<script>
import BarChart from './charts/BarChart.vue'
import LineChart from './charts/LineChart.vue'

export default {
    name: 'Dashboard',
    data() {
        return {
            title:'Dashboard'
        }
    },
    components: {
        BarChart,
        LineChart
    },

    methods: {
        
    },


}
</script>

<style scoped>
    #itemsList {
        width: 100%;
        max-width: 70%;
        margin: 0px;
        padding: 0 5px;
        box-sizing: border-box;
    }
    ul {
        display: flex;
        flex-wrap: wrap;
        list-style-type: none;
        padding: 0;
    }
    li {
        flex-grow: 1;
        flex-basis: 300px;
        text-align: center;
        padding: 10px;
        border: 1px solid #222;
        margin: 10px;
    }
    img {
        width: 135px;
        height: 135px;
    }

    #price {
        font-size: 30px;
    }

    #itemName {
        font-size: 30px;
    }

    #shoppingBasket {
        position: absolute;
        top: 35%;
        left: 78%;
    }

</style>
