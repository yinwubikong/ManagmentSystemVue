<template>
    <div class="main_top">
        <div class="main_top_l">
            <h2>CRM管理后台</h2>
        </div>
        <div class="main_top_r">
            <div class="mtr_name">
                <span>名字</span>
            </div>
            <select name="personstatus" id="personstatus" class="personstatus">
                <option value="修改密码"></option>
                <option value="退出"></option>
            </select>
        </div>
    </div>
    <div class="container">
        <div class="row">

        </div>
    </div>
</template>

<script>

    export default {
        data () {
            return {
                msg: '我是home页'
            }
        },
        created() {

        },
        mounted() {
            this.console()
        },
        methods: {
            console() {
                console.log(1)
            }
        }
    }
</script>

<!--添加 scoped 属性后 当前页面的样式只在此组件生效，不会影响全局同class样式-->
<style scoped>
    .main_top{

    }
    .main_top .main_top_l{

    }
    .main_top .main_top_l h2{

    }
    .main_top .main_top_r{

    }
    .main_top .main_top_r .mtr_name{

    }
    .main_top .main_top_r .mtr_name span{

    }
    .main_top .main_top_r .personstatus{
        
    }



















</style>
