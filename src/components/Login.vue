<template>
    <el-form ref="form" :model="form" label-width="80px">
    <el-form-item label="用户名">
        <el-input v-model="form.name"></el-input>
    </el-form-item>
    <el-form-item label="密码">
        <el-input placeholder="请输入密码" v-model="form.password" show-password></el-input>
    </el-form-item>
    <el-form-item>
        <el-button type="primary" @click="onSubmit">登录1</el-button>
    </el-form-item>
    </el-form>
</template>

<script>
 export default {
    data() {
        return {
            form: {
                name: '',
                password:'',
                region: '',
                date1: '',
                date2: '',
                delivery: false,
                type: [],
                resource: '',
                desc: ''
            }
        }
    },    
    methods: {
      onSubmit() {
        console.log('submit!');
      }
    }
  };
</script>

<style>
</style>
