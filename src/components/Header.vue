<template> 
    <div>
        <ul>
            <li>
                <router-link to="/" exact>Home</router-link>
            </li>
            <li>
                <router-link to="/Orders" exact>Orders</router-link>
            </li>
            <li>
                <router-link to="Dashboard" exact>Dashboard</router-link>
            </li>
        </ul>
    </div> 
</template>

<script>
export default {
    data() {
        return {
            name: "Orders"
        }
    }
}
</script>

<style scoped>
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
</style>