<template>
    <div class="home">
        <htmlHeader :title="'中消在线'"></htmlHeader>
        <nav id="secondary-header" class="navbar" role="navigation">
            <div class="container">
                <ul class="nav navbar-nav">
                    <li><a href="http://www.zxzx119.com">首页</a></li>
                    <li><a href="http://www.zxzx119.com/article-news-1.html">热点新闻</a></li>
                    <li><a href="http://www.zxzx119.com/article-wiki-1.html">政策法规</a></li>
                    <li><a href="http://www.zxzx119.com/article-knowall-1.html">消防百科</a></li>
                    <li><a href="http://www.zxzx119.com/article-supervision-1.html">监督举报</a></li>
                    <li><a href="http://www.zxzx119.com/article-onlineEdu-1.html">教育培训</a></li>
                    <li><a href="http://www.zxzx119.com/article-savezx-1.html">中消救援</a></li>
                </ul>
            </div>
        </nav>
        <div id="advertisement" class="">
            <div id="carousel-advertisement" class="carousel slide" data-ride="carousel">
                <ol class="carousel-indicators">
                    <li data-target="#carousel-advertisement" data-slide-to="0" class="active"></li>
                    <li data-target="#carousel-advertisement" data-slide-to="1" class=""></li>
                </ol>
                <div class="carousel-inner">
                    <div class="item active">
                        <div class="banner-bg" style="">
                            <div class="container">
                                <div class="banner-text">
                                    <div class="solgn center-block">
                                        百强房企用户首选的消防信息服务平台
                                    </div>
                                    <div>
                                        <span class="nufangjianhei">服务热线</span> : 400-1919-119
                                        <br> (周一至周五9:00-17:00，节假日顺延)
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="item">
                        <div class="banner-bg">
                            <div class="container">
                                <div class="banner-text">
                                    <div class="solgn center-block">
                                        百强房企用户首选的消防信息服务平台
                                    </div>
                                    <div>
                                        <span class="nufangjianhei">服务热线</span> : 400-1919-119
                                        <br> (周一至周五9:00-17:00，节假日顺延)
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div id="settled" class="banner-bg v-outter-table" style="">
            <div class="v-table-cell">
                <div class="container">
                    <div class="row">
                        <div class="col-sm-8">
                            <img src="~assets/img/settled-gif.gif" alt="" class="img-responsive center-block">
                        </div>
                        <div class="col-sm-4">
                            <p>中消在线企业名录是以互联网+模式运营的消防专业平台，汇集全行业大数据，融合产业链优势资源， 为房地产企业、安装施工、材料设备生产等相关企业提供个性化、全过程的咨询服务
                            </p>
                        </div>
                        <a class="btn btn-zxzx btn-lg">我要入驻</a>
                    </div>
                </div>
            </div>
        </div>
        <div id="index-footer">
            <div class="container">
                <div class="contact-way row">
                    <div class="col-sm-8 col-md-6">
                        <i class="iconfont icon-zuoji"></i>服务热线: 400-1919-119
                        <br> &nbsp;&nbsp;&nbsp;&nbsp;（周一至周五9:00-17:00，节假日顺延)
                        <br>
                        <i class="iconfont icon-youjian"></i>邮箱：4001919119@zxzx.com
                    </div>
                    <div class="col-sm-4 col-md-6 text-center">
                        <img src="~assets/img/QRcode.png" alt="" class="img-responsive center-block"> 扫码关注订阅号
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {

    name: 'Home',

    data() {
        return {

        };
    }
};
</script>
<style lang="scss" scoped>
@import '~assets/css/variables.scss';
.home {
    &>div:not(:last-child) {
        border-bottom: 2px solid $white-max;
    }
    #secondary-header.navbar {
    	border-radius: 0px;
        z-index: 0;
        margin: {
            top: -$header-margin;
            bottom: 0px;
        }
        background-color: $black-dark;
        height: auto;
        .container {
            padding: {
                top: $header-margin;
                bottom: $header-margin;
            }
            ;
            ul > li > a {
                color: $white-max;
                font-size: 1.2em;
                font-weight: bold;
                padding: {
                    left: 30px;
                    right: 30px;
                    top: 0px;
                    bottom: 0px;
                }
                ;
                @media (max-width: 992px) {
                    padding: {
                        right: 10px;
                    }
                    ;
                }
            }
            ul > li:hover > a {
                color: $white-dark;
                background-color: transparent;
                font-weight: normal;
            }
        }
    }
    #advertisement {
        .carousel {
            .item:nth-child(1) {
            	.banner-bg{
            		background-image: url(~assets/img/index-banner-01.png);
            	}
                
            }
            .item:nth-child(2) {
                .banner-bg{
            		background-image: url(~assets/img/index-banner-02.png);
            	}
            }
            .banner-bg {
                width: 100%;
                height: 400px;
                .banner-text {
                    font-size: 22px;
                    line-height: 40px;
                    position: absolute;
                    bottom: 70px;
                    left: 50%;
                    width: 774px;
                    margin-left: -387px;
                    padding: 30px;
                    color: $white-max;
                    background-color: rgba(0, 0, 0, .5);
                    .solgn {
                        font-family: nufangjianhei;
                        font-size: 42px;
                        margin-bottom: 30px;
                        color: #fff600;
                        text-shadow: 5px 5px 5px $black-bright;
                    }
                }
            }
        }
    }
    #settled {
        background-image: url(~assets/img/settled.png);
        height: 720px;
        .row {
            position: relative;
        }
        .btn-zxzx {
            font-size: 28px;
            line-height: 55px;
            position: absolute;
            padding:0 20px;
            top: 50%;
            @media (min-width: 768px) {
                right: 70px;
            }
            @media (min-width: 992px) {
                right: 170px;
            }
            @media (min-width: 1200px) {
                right: 270px;
            }
        }
        p {
            font-size: 18px;
            color: $white-max;
            @media (min-width: 768px) {
                margin-left: 14px;
            }
            @media (min-width: 992px) {
                font-size: 20px;
                margin-left: -8px;
            }
            @media (min-width: 1200px) {
                font-size: 22px;
                margin-left: -50px;
            }
        }
    }
    #index-footer {
        font-size: 18px;
        line-height: 40px;
        height: 300px;
        padding-top: 75px;
        color: $white-max;
        background-color: $hot-dark;
        .contact-way {
            padding: 0 10%;
            & > div:first-child {
                border-right: 1px solid $white-max;
            }
            i {
                margin-right: 20px;
            }
        }
    }
}
</style>
