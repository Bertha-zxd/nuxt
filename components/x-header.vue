<template>
    <div class="x-header">
        <div class="h-wrap">
            <div class="w-left">
                <div class="l-logo">
                    <h1>Fairy</h1>
                </div>
                <div class="l-module">
                    <div class="m-item">
                        <span>首页</span>
                    </div>
                </div>
            </div>
            <div class="w-right">
                <div class="r-search">
                    <input type="text" placeholder="搜索更新啦">
                    <i class="iconfont icon-sousuo"></i>
                </div>
                <div class="r-do">
                    <div class="d-item">
                        <i class="iconfont icon-xiezi"></i>
                        <span>写文章</span>
                    </div>
                    <div class="d-item">
                        <span>登录</span>
                        <span>/</span>
                        <span>注册</span>
                    </div>
                    <!-- <div>
                        <span>注销</span>
                    </div> -->
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
.x-header{
   position:fixed;
   top:0;
   left: 0;
   width: 100%;
   background: white;
   border-bottom: 1px solid #f1f1f1;
   z-index: 1000;
   .h-wrap{
       display: flex;
       justify-content: space-between;
       width: 960px;
       height: 60px;
       margin: 0 auto;
        //align-items: center;
       .w-left{
           display: flex;
        //    justify-content: space-between;
           align-items: center;
            .l-logo{
                h1{
                    color: #007fff;
                }
            }
            .l-module{
                .m-item{
                    span{
                        color: #007fff;
                        padding:0 20px;
                        font-size:16px;
                    }
                }
            }
       }
       .w-right{
           display: flex;
           align-items: center;
           .r-search{
            display: flex;  
            height: 30px;
            padding: 0 10px ;
            background: #cccccc;
            font-size: 14px;
            margin-right: 30px;
                input{
                    outline: none;
                    border: 0;
                    background: none;
                    width:90px;
                }
                i{
                    font-size: 20px;
                }
           }
           .r-do{
               display: flex;
               align-items: center;
               color: #007fff;
               font-size: 16px;
               .d-item{
                   display: flex;
                   align-items: center;
                   i{
                        font-size: 20px;
                    }
                    span{
                        &:nth-child(2){
                            padding: 0 10px;
                        }
                    }
                    &:last-child{
                        position:relative;
                        padding-left: 20px;
                        &:before{
                            position: absolute;
                            content: "";
                            width:1px;
                            background:black;
                            top: 50%;
                            transform: translateY(-50%);
                            left: 10px;
                            height: 70%;
                        }
                        // border-left: 1px solid #f1f1f1;
                    }
               }
               
           }
       }
   }
}
</style>
