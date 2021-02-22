<template>
    <div>
        <el-button type="info" @click="loginout">退出</el-button>
    </div>
</template>
<script>
export default {
    methods: {
        //退出登录
        loginout() {
            // 1. 销毁token值
            window.sessionStorage.clear();
            // 2. 重定向到登录页
            this.$router.push('/login');
        }
    }
};
</script>

<style scoped>

</style>