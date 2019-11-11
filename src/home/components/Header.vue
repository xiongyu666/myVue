<template>
  <div class="header">
    <div class="header-con">
      <div class="header-logo">
        <img src="../../assets/logo.png" alt="">
      </div>
      <div class="header-nav">
        <ul>
          <li>
            <div>
              <router-link to="/">首页</router-link>
              <div class="span-border"></div>
            </div>
          </li>
          <li>
            <div>
              <router-link to="/">网站建设</router-link>
              <div class="span-border"></div>
            </div>
            <div class="nav-tobar">

            </div>
          </li>
          <li>
            <div>
              <router-link to="/">微信小程序</router-link>
              <div class="span-border"></div>
            </div>
          </li>
          <li>
            <div>
              <router-link to="/">H5开发</router-link>
              <div class="span-border"></div>
            </div>
          </li>
          <li>
            <div>
              <router-link to="/">平台开发</router-link>
              <div class="span-border"></div>
            </div>
          </li>
          <li>
            <div>
              <router-link to="/">案例</router-link>
              <div class="span-border"></div>
            </div>
          </li>
          <li>
            <div>
              <router-link to="/">方案</router-link>
              <div class="span-border"></div>
            </div>
          </li>
          <li>
            <div>
              <router-link to="/">资讯</router-link>
              <div class="span-border"></div>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'HomeHeader',
    data () {
      return {
        nav: [
          {
            id: "01",
            name: "首页",
            urls: "/"
          },
          {
            id: "02",
            name: "网站建设",
            urls: "/"
          },
          {
            id: "03",
            name: "微信小程序",
            urls: "/"
          },
          {
            id: "04",
            name: "H5开发",
            urls: "/"
          },
          {
            id: "05",
            name: "平台开发",
            urls: "/"
          },
          {
            id: "06",
            name: "案例",
            urls: "/"
          },
          {
            id: "07",
            name: "方案",
            urls: "/"
          },
          {
            id: "08",
            name: "资讯",
            urls: "/"
          },
          {
            id: "09",
            name: "关于",
            urls: "/"
          },
        ]
      }
    },
    components:{

    }
  }
</script>

<style lang="less" scoped>
  .header {
    background: rgba(0,0,0,.5);
    width: 100%;
    position: fixed;
    top: 0;
    z-index: 9999;
    .header-con {
      width: 83.33%;
      margin: 0 auto;
      .header-logo {
        float: left;
        margin-top: 20px;
      }
      .header-nav {
        float: right;
        ul{
          overflow: hidden;
          li{
            float: left;
            padding: 0 20px;
            .nav-tobar{
              position: absolute;
              left: 0;
              width: 100%;
              height: 300px;
              background: #fff;
              display: none;
            }
            .span-border{
              width: 0;
              bottom: 0;
              transition: all 0.5s;
              height: 2px;
              background: #0aa3f3;
            }
            a{
              padding: 36px 0 34px 0;
              color: #fff;
              text-decoration: none;
              display: block;
            }
          }
          li:hover .span-border{
            width: 100%;
          }
          li:hover a{
            color: #0aa3f3;
          }
        }
      }
    }
  }
</style>
