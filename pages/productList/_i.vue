<template>
    <div>
        <p>产品1</p>
        <span>产品2</span>
    </div>
</template>

<script>
    export default {
        name: "index",
        mounted() {
            this.$store.commit('mo1/todos/say')
            this.$store.commit('say')
        }
    }
</script>

<style rel="stylesheet/scss" lang="scss" scoped>
    @import "./assets/scss/common/_mixin";
    div{
        p{
            color: $c-help;
            //@include clearfix;
            //@include ellipsis;
        }
        span{
            color: red;
        }
    }
</style>
