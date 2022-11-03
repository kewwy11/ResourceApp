<template>
 <ul>
        <list-resources v-for="res in resources" 
        :key="res.id" 
        :id="res.id"
        :title="res.title" 
        :description="res.description" 
        :link="res.link">
        </list-resources>
    </ul>
</template>

<script>
    import ListResources from './ListResources.vue'


    export default{
        components:{
        ListResources
    },
        inject:['resources']
    }
</script>

<style>
    ul {
  list-style: none;
  margin: 0;
  padding: 0;
  margin: auto;
  max-width: 40rem;
}
</style>