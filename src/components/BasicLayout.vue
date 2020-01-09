<template>
  <div class="container">
    <el-container class="h100" v-if="pc">
      <el-container class="sider-pc">
        <Sider />
      </el-container>
      <el-container class="content-pc">
        <el-header class="page-header" height="64px">
          <Header></Header>
        </el-header>
        <el-main class="page-mainer">
          <router-view></router-view>
        </el-main>
        <Footer />
      </el-container>
    </el-container>
    <swiper class="mobile h100" v-else :options="swiperOption" ref="mySwiper">
      <swiper-slide class="mobile-item slide">
        <div class="slide-container">
          <Sider />
          <div class="swiper-tips">
            <div class="tips-cn">左右滑动</div>
            <div class="more">
              <div class="more-ball"></div>
            </div>
          </div>
        </div>
      </swiper-slide>
      <swiper-slide class="mobile-item">
        <el-header class="page-header" height="64px">
          <Header></Header>
        </el-header>
        <el-main class="page-mainer">
          <router-view></router-view>
        </el-main>
        <Footer />
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
import Header from "./BasicLayoutHeader.vue";
import Footer from "./BasicLayoutFooter.vue";
import Sider from "./BasicLayoutSider.vue";

export default {
  data() {
    return {
      pc: true,
      swiperOption: {
        loop: true
      }
    };
  },
  created() {
    window.addEventListener("pageshow", this.mobileFunc);
    window.addEventListener("resize", this.mobileFunc);
  },
  methods: {
    mobileFunc() {
      let width = document.documentElement.clientWidth;
      if (width < 720) {
        this.pc = false;
      } else if (width >= 720) {
        this.pc = true;
      }
    }
  },
  components: {
    Header,
    Footer,
    Sider
  }
};
</script>

<style type="text/css" lang="less">
@media screen and (max-width: 720px) {
  .page-header {
    padding: 0 10px;
  }
}
.h100 {
  height: 100vh;
}
.mobile {
  width: 100%;
  height: 100%;
  .mobile-item {
    width: 100%;
    height: auto;
  }
  .slide {
    background-color: #17a8aa;
  }
  .slide-container {
    height: 100vh;
    position: relative;
    .swiper-tips {
      position: absolute;
      bottom: 10px;
      left: 50%;
      transform: translateX(-50%);
      font-size: 13px;
      color: #fff;
      display: flex;
      align-items: center;
      .more {
        border: 2px solid #fff;
        height: 6px;
        width: 25px;
        border-radius: 12px;
        padding: 7px;
        display: block;
        position: relative;
        margin-left: 8px;
        .more-ball {
          position: absolute;
          border: 1px solid #fff;
          background-color: #fff;
          height: 8px;
          width: 8px;
          border-radius: 20px;
          top: 26%;
          animation: slideiconleft 2s 1s linear infinite;
        }
        @keyframes slideiconleft {
          0% {
            opacity: 1;
            left: 70%;
          }
          100% {
            opacity: 0;
            left: 10%;
          }
        }
      }
    }
  }
}
.sider-pc {
  width: 25%;
}
.content-pc {
  width: 75%;
}
.page-header {
  box-shadow: 6px 2px 8px #eae5c9;
  position: relative;
  z-index: 10;
  height: 64px;
  .page-header-title {
    font-size: 20px;
  }
}

.page-sider {
  position: relative;
  background-color: #17a8aa;
  box-shadow: 2px 0 8px 0 rgba(29, 35, 41, 0.05);
  .el-menu {
    border-right: none;
  }
}

.page-mainer {
  padding: 0;
}
</style>
