<template>
    <div>
        <div class="main_top clearfix">
            <div class="main_top_l">
                <h2>CRM管理后台</h2>
            </div>
            <div class="main_top_r">
                <div class="mtr_name">
                    <span>名字</span>
                </div>
                <select name="personstatus" id="personstatus" class="personstatus">
                    <option value="0">修改密码</option>
                    <option value="1">退出</option>
                </select>
            </div>
        </div>
        <div class="container-fluid">
            <div class="row">
                <div class="col-md-2 main_left" ref="homePage">
                    <ul class="ml_box">
                        <li>
                            <a href="#">aaa</a>
                        </li>
                        <li>
                            <a href="#">bbb</a>
                        </li>
                        <li>
                            <a href="#">ccc</a>
                        </li>
                    </ul>
                </div>
                <div class="col-md-10 main_right">

                </div>
            </div>
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


//            document.getElementsByClassName("main_right")[0].style.height=(document.documentElement.clientHeight - 60) + 'px'
        },
        methods: {


        },
        watch:{

        }
    }
</script>

<!--添加 scoped 属性后 当前页面的样式只在此组件生效，不会影响全局同class样式-->
<style scoped>
    *{
        margin: 0;
        padding: 0;
    }
    ul,ol,dl,li{
        list-style: none;
    }
    html,body,:root{
        height: 100%;
    }
    .main_top{
        height: 60px;
        background: #777a7d;
    }
    .main_top .main_top_l{
        float: left;
        height: 60px;
        width: 200px;
        line-height: 60px;

    }
    .main_top .main_top_l h2{
        font-size: 28px;
        color: #333333;
        line-height: 58px;
        margin-left: 20px;
    }
    .main_top .main_top_r{
        float: right;
        height: 60px;
        font-size: 0;
    }
    .main_top .main_top_r .mtr_name{
        height: 40px;
        margin: 10px 20px 10px 0;
        line-height: 40px;
        color: #333333;
        display: inline-block;
        font-size: 16px;
    }
    .main_top .main_top_r .mtr_name span{

    }
    .main_top .main_top_r .personstatus{
        font-size: 14px;
        height: 30px;
        appearance:none;
        -moz-appearance:none;
        -webkit-appearance:none;
        background: dimgrey;
        padding-right: 16px;
        margin-right: 20px;
    }
    .main_left{
        /*height: 100%;*/
        /*min-height: 500px;*/
        background: #4d5e70;
        height: calc(100vh - 60px);
    }
    .ml_box{

    }
    .ml_box li{
        height: 40px;
        font-size: 20px;
        margin-bottom: 6px;
    }
    .main_right{
        height: calc(100vh - 60px);
        /*文章注解https://www.w3cplus.com/css3/how-to-use-css3-calc-function.html*/
    }

</style>
