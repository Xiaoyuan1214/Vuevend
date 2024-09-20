<template>
  <ItemComponent
    v-for="item in $store.state.products"
    v-bind:key="item.id"
    v-bind:item="item"
  ></ItemComponent>
</template>

<script>
import ItemComponent from '../components/ItemComponent.vue'

export default {
  components:{ItemComponent}
}
</script>

<style>

</style>