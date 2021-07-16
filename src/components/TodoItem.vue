<template>
  <li class="item" @click="handleDelete">{{ content }}</li>
</template>

<script>
export default {
  props: ["content", "index"],
  methods: {
    handleDelete: function () {
      // console.log(this.index);
      this.$emit("delete", this.index);
    },
  },
};
</script>



<style scoped>
/* scoped 属性可以保证样式为局部样式 */
.item {
  color: green;
}
</style>>

