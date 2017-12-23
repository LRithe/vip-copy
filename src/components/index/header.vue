<template>
    <div>
        <div id="nav-top-bar">
            <div class="container clearfix">
                <div id="nav-top-bar-left">
                    <div id="sel-area">
                        <span>四川</span>
                        <i class="ico-dis"></i>
                    </div>
                </div>
                <ul id="nav-top-bar-right">
                    <li class="top-menu"><a href="#">请登录</a></li>
                    <li class="top-menu"><a href="#">注册</a></li>
                    <li class="top-menu"><a href="#"><span></span>签到有礼</a></li>
                    <li class="top-menu"><a href="#">我的订单</a></li>
                    <li class="top-menu te-mai">
                        <a href="#" class="top-menu-btn">
                            我的特卖<i class="ico-dis"></i>
                        </a>
                        <ul id="te-mai-menu" class="list-menu">
                            <li>
                                <a href="#">品牌特卖</a>
                            </li>
                            <li>
                                <a href="#">品牌特卖</a>
                            </li>
                            <li>
                                <a href="#">品牌特卖</a>
                            </li>
                        </ul>
                    </li>
                    <li class="top-menu"><a href="#" class="top-menu-btn">会员俱乐部<i class="ico-dis"></i></a></li>
                    <li class="top-menu"><a href="#" class="top-menu-btn">客户服务<i class="ico-dis"></i></a></li>
                    <li class="top-menu"><a href="#"><span></span>手机版</a></li>
                    <li class="top-menu"><a href="#" class="top-menu-btn">更多 <i class="ico-dis"></i></a></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
  export default {
    name: 'index-header'
  }
</script>

<style scoped>
    #nav-top-bar {
        background-color: #f5f5f5;
        color: rgba(85, 85, 85, 0.65);
    }

    .container {
        width: 1170px;

        /* 块级元素居中*/
        margin-left: auto;
        margin-right: auto;

        font-size: 12px;
        height: 30px;
        line-height: 30px;
    }

    #nav-top-bar-left {
        float: left;
        position: relative;
    }

    #sel-area {
        cursor: pointer;
    }

    #sel-area:hover .ico-dis, .top-menu:hover .ico-dis {
        border-color: transparent transparent #999 transparent;
        top: 7px;
    }

    #nav-top-bar-right {
        float: right;
        list-style: none;
    }

    .top-menu {
        float: left;
        cursor: pointer;
        margin-right: 5px;
    }

    .top-menu .ico-dis {
        right: 7px;
    }

    .top-menu a {
        display: inline-block;
        color: rgba(85, 85, 85, 0.65);
        padding: 0 13px;
        position: relative;
        height: 30px;
        border: 1px solid transparent;
    }

    .top-menu:not(:last-child):after {
        content: '/';
        display: inline-block;
    }

    .te-mai {
        position: relative;
    }

    .top-menu .top-menu-btn {
        padding-right: 20px;
    }

    .top-menu:hover .top-menu-btn {
        background-color: white;
        border: 1px solid #ccc;
        border-bottom: none;
        z-index: 2;
        box-sizing: content-box;
    }

    .list-menu {
        display: none;
        position: absolute;
        background-color: white;
        border: 1px solid #ccc;
        width: 130px;
        top: 30px;
        z-index: 1;
    }

    .top-menu:hover .list-menu {
        display: block;
    }
</style>