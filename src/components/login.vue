<template>
  <form>
    <label>{{data_user}}</label>
    <input type="text"/>
    <label>{{data_pswd}}</label>
    <input type="password"/>
    <input type="submit" v-on:click="login" value="登录"/>
  </form>
</template>

<script>
export default {
  data () {
    return {
      data_user: '用户名',
      data_pswd: '密码'
    }
  },
  methods: {
    login: function () {
      this.$router.push({
        path: '/'
      })
    }
  }
}
</script>

<style>
  h1, h2 {
    font-weight: normal;
  }
</style>
