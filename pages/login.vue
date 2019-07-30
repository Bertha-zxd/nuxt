<template>
    <div class="login">
        <div class="l-box">
            <div class="b-top">
                <div class="t-title">
                    <h2>账号密码登录</h2>
                </div>
                <div class="t-from">
                    <input type="text" placeholder="账号">
                    <input type="password" placeholder="密码">
                </div>
                <div class="t-auto">
                    <input type="checkbox">
                    <span>自动登录</span>
                </div>
                <div class="t-btn">
                    <span>登陆</span>
                </div>
                <div class="t-forget">
                    <span>忘记密码?</span>
                </div>
            </div>
            <div class="b-bottom">
                <div class="b-left">
                    <span>第三方登陆</span>
                    <i class="iconfont icon-weixin"></i>
                </div>
                <div class="b-right">
                    <span>立即注册</span>
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
.login{
    position: absolute;
    top: 0;
    bottom: 0;
    width: 100%;
    background: url(https://www.link-nemo.com/forumlib/images/banner02.jpg) center no-repeat;
    background-size: cover;
    .l-box{
        position:absolute;
        top:50%;
        transform: translateY(-50%);
        right: 23%;
        .b-top{
            
            width: 350px;
            padding: 0 20px;
            background:white;
            .t-title{
                height: 100px;
                display: flex;
                align-items: center;
            }
            .t-from{
                display: flex;
                flex-flow: column;
                input{
                    padding: 10px;
                    border:1px solid #f4f5f5;
                    &:nth-child(2){
                        border-top:none;
                    }
                }
            }
            .t-auto{
                height: 54px;
                display: flex;
                align-items: center;  
            }
            .t-btn{
                height: 40px;
                background:#00a7eb;
                display: flex;
                justify-content: center;
                align-items: center;
                span{
                    color: white;
                }
            }
            .t-forget{
                height: 50px;
                display: flex;
                align-items: center;
            }
        }
        .b-bottom{
            width: 350px;
            height: 60px;
            padding: 0 20px;
            background:#f3f8ff;
            display: flex;
            justify-content: space-between;
            align-items: center;
            color: #00a7eb;
            .b-left{
                span{
                    margin-right: 30px;
                }
            }
        }
    }
}
</style>
