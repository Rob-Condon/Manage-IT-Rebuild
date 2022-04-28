<template>
  <div class="flex md6 mb-4">
    <router-link to="/">
      <div class="item" @mouseover="hovering = true" @mouseleave="hovering = false">
        <h3 class="primary mb-1 link-item" >{{title}} <va-icon class="material-icons" :size="16" v-show="hovering" >arrow_forward</va-icon> </h3>
        <p class="secondary text-size-small">{{description}}</p>
      </div>
    </router-link>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    description: String
  },
  data() {
    return {
      hovering: false
    }
  },
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Service"
}
</script>

<style scoped>
.item:hover {
  cursor: pointer;
}


</style>