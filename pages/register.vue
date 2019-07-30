<template>
    <div class="register">
        <div class="r-header">
            <div class="h-wrap">
                <div class="w-left">
                    <div class="w-logo">
                        <h1>Fairy</h1>
                    </div>
                    <div class="w-title">
                        <span>注册账号</span>
                    </div>
                </div>
                <div class="w-right">
                    <div class="r-desc">
                        <span>我已注册，现在</span>
                    </div>
                    <div class="r-btn">
                        <span>登陆</span>
                    </div>
                </div>
            </div>
        </div>
        <div class="r-content">
            <div class="c-wrap">
                <div class="c-field">
                    <div class="f-item">
                        <div class="i-left">
                            <span>用户账号</span>
                        </div>
                        <div class="i-right">
                            <input type="text" placeholder="请输入账号">
                        </div>
                    </div>
                    <div class="f-item">
                        <div class="i-left">
                            <span>用户密码</span>
                        </div>
                        <div class="i-right">
                            <input type="password" placeholder="请输入密码">
                        </div>
                    </div>
                    <div class="f-item">
                        <div class="i-left">
                            <span>密码确认</span>
                        </div>
                        <div class="i-right">
                            <input type="password" placeholder="请确认密码">
                        </div>
                    </div>
                    <div class="f-item">
                        <div class="i-left">
                            <span>邀请码</span>
                        </div>
                        <div class="i-right">
                            <input type="text">
                            <span>没有邀请码？</span>
                        </div>
                    </div>
                </div>
                <div class="c-law">
                    <div class="l-check">
                        <div class="c-checkbox">
                            <input type="checkbox">
                        </div>
                        <div class="c-item">
                            <span>阅读并接受</span>
                            <a href="">《fairy使用手册》</a>
                        </div>
                    </div>
                    <div class="l-btn">
                        <span>注册</span>
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
.register{
    .r-header{
        position:fixed;
        top:0;
        left: 0;
        width: 100%;
        display: flex;
        justify-content: center;
        .h-wrap{
            width:1200px;
            height: 80px;
            box-shadow: 0 0 10px 0 rgba(2, 2, 2, 0.2); 
            display: flex;
            justify-content: space-between;
            padding:20px 80px;
            .w-left{
                display: flex;
                align-items: center;
                .w-title{
                    margin-left: 20px;
                    span{
                        font-size: 16px;
                    }
                }
            }
            .w-right{
                display: flex;
                align-items: center;
                .r-btn{
                    width: 60px;
                    height: 30px;
                    background:#00a7eb;
                    margin-left: 10px;
                    border-radius: 3px;
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    span{
                        color: white;
                    }
                }
            }
        }
    }
    .r-content{
        position:absolute;
        top:150px;
        left: 200px;
        .c-wrap{
            .c-field{
                
                .f-item{
                    display: flex;
                    align-items: center;
                    margin-bottom: 25px;
                    .i-left{
                        width: 60px;
                        font-size: 14px;
                        font-weight: bold;
                        display: flex;
                        justify-content: flex-end;
                    }
                    .i-right{
                        width:350px;
                        padding-left: 10px;
                        display: flex;
                        align-items: center;
                        input{
                           flex: 1;
                           height:40px ;
                        }
                        span{
                            margin-left: 10px;
                            color: #00a7eb;
                        }
                    }
                }
            }
        }
        .c-law{
            position: relative;
            .l-check{
                display: flex;
                align-items: center;
                margin-left: 60px;
                vertical-align: middle;
            }
            .l-btn{
                position: absolute;
                right: 0;
                width: 350px;
                height: 50px;
                margin-top:20px;
                background: #00a7eb;
                display: flex;
                align-items: center;
                justify-content: center;
                span{
                    color: white;
                }
            }
        }
    }
}
</style>
