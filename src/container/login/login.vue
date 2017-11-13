<template>
  <div>
    <Field label="用户" placeholder="请输入用户名" v-model="username"></Field>
    <Blank />
    <Field label="密码" placeholder="请输入密码" v-model="password"></Field>
    <Blank />
    <Button type="primary" style="width:100%">登录</Button>
    <Blank />
    <Button type="primary" style="width:100%" @click="register">注册</Button>
  </div>
</template>
<script>
import { Field, Button } from 'mint-ui'
import Blank from '../../components/blank/blank'
export default {
  data () {
    return {
      username: '',
      password: ''
    }
  },
  components: {
    Field,
    Button,
    Blank
  },
  methods: {
    register() {
      console.log(1)
    }
  }
}
</script>
