<!--
 * @Author: your name
 * @Date: 2020-05-05 15:03:37
 * @LastEditTime: 2020-05-05 16:23:37
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
 * @FilePath: /learn-basic/vue-source-code/src/components/form/input.vue
 -->

<template>
  <div>
    <input :value="value" @input="onInput" />
  </div>
</template>

<script>
export default {
  props: {
    value: {
      type: String,
      default: ""
    }
  },
  methods: {
    onInput(e) {
      this.$emit("input", e.target.value);
    }
  }
};
</script>

<style lang="scss" scoped>
</style>
