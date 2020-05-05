<!--
 * @Author: your name
 * @Date: 2020-05-05 15:03:48
 * @LastEditTime: 2020-05-05 18:53:22
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
 * @FilePath: /learn-basic/vue-source-code/src/components/form/index.vue
 -->
<template>
  <div>
    <p>Element表单</p>
    <hr />
    <k-form>
      <k-formItem label="用户名" prop="username">
        <k-Input />
      </k-formItem>
      <k-formItem label="密码" prop="password">
        <k-Input />
      </k-formItem>
      <k-formItem>
        <button @click="submitForm('loginForm')">提交</button>
      </k-formItem>
    </k-form>
  </div>
</template>

<script>
import KForm from "./Form";
import KFormItem from "./FormItem";
import KInput from "./Input";
export default {
  components: {
    KForm,
    KFormItem,
    KInput
  }
  // props: {
  //   submitForm: type => {
  //     console.log("submitForm", type);
  //   }
  // }
};
</script>

<style lang="scss" scoped>
</style>