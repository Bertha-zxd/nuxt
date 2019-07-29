<template>
    <div class="c-right">
        <div class="r-section r-section-login">
            <div class="l-title">
                <span>FAIRY - blog.fairy.cn</span>
            </div>
            <div class="l-desc">
                <span>一个分享知识学习的好地方</span>
            </div>
            <div class="l-form">
                <div class="f-item">
                    <span>账号</span>
                </div>
                <div class="f-item">
                    <span>密码</span>
                </div>
            </div>
            <div class="l-btn">
                <span>立即注册</span>
            </div>
            <div class="l-third">
                <div class="t-left">
                    <span>第三方登陆：</span>
                </div>
                <div class="t-right">
                    <div class="r-item">
                        <i class="iconfont icon-weixin"></i>
                    </div>
                    <div class="r-item">
                        <i class="iconfont icon-github"></i>
                    </div>
                </div>
            </div>
        </div>
        <div class="r-section r-section-tag">
            <div class="t-title">
                <span>热门标签</span>
                <span>查看全部</span>
            </div>
            <div class="t-content">
                <div class="c-item">
                    <span>DevOps</span>
                </div>
            </div>
        </div>
        <div class="r-section r-section-book">
            <div class="b-title">
                <div class="t-left">
                    <span>专题</span>
                </div>
                <div class="l-right">
                    <i class="iconfont icon-back"></i>
                    <i class="iconfont icon-next"></i>
                </div>
            </div>
            <div class="b-content">
                <div class="c-item">
                    <img src="@/assets/book_1.jpg">
                    <div>
                        <span>keyteo项目快速入门</span>
                        <span>keyteo</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="less">
.c-right{
    .r-section{
        width: 240px;
        background: white;
        &-login{
            display: flex;
            flex-flow: column;
            justify-content: center;
            padding:20px;
            .l-title{
                span{
                    font-size: 14px;
                    font-weight: bold;
                }
            }
            .l-desc{
                span{
                    font-size: 14px;
                    color: #b2bac2;
                }
            }
            .l-form{
                .f-item{
                    width:100%;
                    height: 36px;
                    background:#b2bac2;
                    margin-top:10px;
                    padding-left:10px;
                    display: flex;
                    align-items: center;
                    span{
                        font-size: 14px;

                    }
                }
            }
            .l-btn{
                width:100%;
                height:36px;
                margin-top:10px;
                background: #007fff;
                display: flex;
                justify-content: center;
                align-items: center;
                border-radius: 5px;
                span{
                    color: white;
                }
            }
            .l-third{
                display: flex;
                align-items: center;
                margin-top: 10px;
                .t-right{
                    display: flex;
                    .r-item{
                        &:nth-child(1){
                            margin-right: 10px;
                        }
                    }
                }
            }
        }
        &-tag{
            margin-top: 30px;
            .t-title{
                padding: 10px 20px;
                display: flex;
                justify-content: space-between;
                border-bottom: 1px solid #b2bac2;
                span{
                    font-size: 14px;
                    &:nth-child(2){
                        color: #007fff;
                    }
                }
            }
            .t-content{
                padding:20px;
                display: flex;
                .c-item{
                    // width: 60px;
                    padding: 0 10px;
                    height: 30px;
                    background: #b2bac2;
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    border-radius: 15px;
                    span{
                        font-size: 14px;
                    }
                }
            }
        }
        &-book{
            margin-top: 30px;
            .b-title{
                padding: 10px 20px;
                display: flex;
                justify-content: space-between;
                border-bottom: 1px solid #b2bac2;
                span{
                    font-size: 14px;
                }
            }
            .b-content{
                .c-item{
                    padding: 20px 10px;
                    display: flex;
                    img{
                        width: 52px;
                        height: 72px;
                    }
                    div{
                        margin-left: 10px;
                        display: flex;
                        flex-flow: column;
                        span{
                            font-size: 14px;
                            &:nth-child(2){
                                color: red;
                            }
                        }
                    }
                }
            }
        }
    }
}
</style>
