<template>
  <div class="index">
    <x-header></x-header>
    <div class="h-tab">
      <div class="t-warp">
        <div class="w-item">
          <span class="i-list i-list-active">今日热门</span>
          <span class="i-list">前端</span>
          <span class="i-list">后端</span>
          <span class="i-list">嵌入式</span>
          <span class="i-list">人工智能</span>
        </div>
      </div>
    </div>
    <div class="i-content">
      <div class="c-left">
        <div class="l-article">
          <div class="a-item a-item-active">
            <span>推荐</span>
          </div>
          <div class="a-item">
            <span>最新</span>
          </div>
          <div class="a-item">
            <span>热门</span>
          </div>
        </div>
        <div class="l-list">
          <div class="l-item">
            <div class="i-info">
              <span>文章</span>
              <span>bertha</span>
              <span>Javascript</span>
            </div>
            <div class="i-title">
              <span>《Vue.js开发技巧》</span>
              <span>Vuejs静态部署</span>
            </div>
            <div class="i-do">
              <div class="d-btns">
                <div class="b-item">
                  <i class="iconfont icon-like"></i>
                  <span>1</span>
                </div>
                <div class="b-item">
                  <i class="iconfont icon-pinglun"></i>
                  <span>1</span>
                </div>
              </div>
            </div>
            <div class="i-img">
            </div>
          </div>
        </div>
        <x-footer></x-footer>
      </div>
      <c-right></c-right>
    </div> 
  </div>
</template>

<script>
import xHeader from '~/components/x-header'
import xFooter from '~/components/x-footer'
import cRight from '~/components/c-right'
export default {
  components: {
    xHeader,
    xFooter,
    cRight
  },
  data(){
    return{
      
    }
  }
}
</script>

<style lang="less">
.index{
  background: #f4f5f5;
  .h-tab{
    position: fixed;
    top:61px;
    left: 0;
    z-index: 999;
    width: 100%;
    background: white;
    box-shadow: 0px 0px 10px 0px rgba(2, 2, 2, 0.2); 
    .t-warp{
      width: 960px;
      height: 46px;
      margin:0 auto;
      display: flex;
      .w-item{
        display: flex;
        align-items: center;
        .i-list{
          font-size: 14px;
          padding: 0 10px;
          &-active{
            color: aqua;
          }
          &:hover{
            color: aqua;
          }
        }
       
      }
    }
  }
  .i-content{
    display: flex;
    width: 960px;
    margin: 0 auto;
    padding-top:126px;
    .c-left{
      display: flex;
      flex-flow: column;
      width:700px;
      margin-right: 20px;
      .l-article{
        width: 100%;
        height: 45px;
        background: white;
        display: flex;
        align-items: center;
        padding:0 20px;
        border-bottom: 1px solid #ccc;
        .a-item{
          display: flex;
          span{
            font-size: 14px;
          }
          &-active {
            span {
                color: aqua;
            }
          }
          &:hover{
            color: aqua;
          }
          &:not(:first-child){
            position: relative;
            margin-left: 30px;
            &:before{
              position: absolute;
              width: 1px;
              height: 70%;
              content: "";
              top: 50%;
              transform: translateY(-50%);
              left: -15px;
              background: black;
            }
          }
        }
      }
      .l-list{
        .l-item{
          padding:20px 100px 20px 20px;
          background: white;
          // height: 126px;
          .i-info{
            display: flex;
            span{
              font-size: 14px;
              &:nth-child(1){
                color: aqua;
              }
              &:not(:first-child){
                position: relative;
                padding-left:20px;
                color: #ccc;
                &::before{
                  position: absolute;
                  content: "/";
                  top:50%;
                  transform: translateY(-50%);
                  left: 10px;
                }
              }
            }
          }
          .i-title{
            margin-top: 10px;
            span{
              font-size: 16px;
              font-weight: bold;
            }
          }
          .i-do{
            margin-top: 20px;
            .d-btns{
              display: flex;
              align-items: center;
              .b-item{
                display: flex;
                align-items: center;
                justify-content: center;
                width: 50px;
                height: 24px;
                border:1px solid #ccc;
              }
            }
          }
        }
      }
    }
  }
}
</style>
