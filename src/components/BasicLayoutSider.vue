<template>
  <el-aside class="page-sider" style="width:100%;height:100%">
    <div class="user-info">
      <div class="user-avatar">
        <img class="user-avatar-png" src="@/assets/me.jpg" />
      </div>
      <p class="user-name">旷奇</p>
      <p class="user-status">{{ typist }}</p>
    </div>
    <div class="user-info">
      <div class="user-info-title">个人信息</div>
      <div class="user-info-text">
        <i class="el-icon-trophy"></i>
        <span>毕业学校：湖南信息职业技术学院</span>
      </div>
      <div class="user-info-text">
        <i class="el-icon-present"></i>
        <span>出生年月：1997.10.20</span>
      </div>
      <div class="user-info-text">
        <i class="el-icon-position"></i>
        <span>意向城市：广州、深圳</span>
      </div>
      <div class="user-info-text">
        <i class="el-icon-mobile-phone"></i>
        <span>联系方式：13112808045（同微信号）</span>
      </div>
      <div class="user-info-text">
        <i class="el-icon-wind-power"></i>
        <span>应聘职位：前端研发工程师</span>
      </div>
      <div class="user-info-text">
        <i class="el-icon-bank-card"></i>
        <span>期望月薪：8～12k</span>
      </div>
    </div>
    <div class="user-info">
      <div class="user-info-title">实习经历</div>
      <div class="user-info-text">
        <i class="el-icon-office-building"></i>
        <span>2019 广州市扎克斯科技 - 前端工程师</span>
      </div>
    </div>
  </el-aside>
</template>

<script>
export default {
  data() {
    return {
      typist: "",
      text_1: "我是一个程序员",
      text_2: "不，我是一名前端工程师",
      index: 1,
      change: true
    };
  },
  created() {
    setInterval(() => {
      let i = this.index;
      this.typing(i);
      this.index += 1;
    }, 500);
  },
  methods: {
    typing(i) {
      let text_1 = this.text_1;
      let text_2 = this.text_2;
      let text = "";
      this.change ? (text = text_1) : (text = text_2);
      if (i <= text.length) {
        this.typist = text.slice(0, i) + "_";
      } else {
        this.index = 1;
        this.change = !this.change;
      }
    }
  }
};
</script>

<style type="text/css" lang="less">
::-webkit-scrollbar {
  width: 10px;
  background-color: #c0c0c0;
}
::-webkit-scrollbar-thumb {
  background-color: #808080;
  border-radius: 20px;
}
::-webkit-scrollbar-thumb:hover {
  background-color: #808080;
}
::-webkit-scrollbar-thumb:active {
  background-color: #a0522d;
}
::-webkit-scrollbar-thumb:window-inactive {
  background-color: #808080;
}
.page-sider {
  position: relative;
  box-shadow: 2px 0 8px 0 rgba(29, 35, 41, 0.05);
  transition: all 0.2s ease;
  width: 100%;
  color: #fff;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-top: 20px;
  .user-info {
    margin: 20px 0;
    .user-info-title {
      font-size: 16px;
      font-weight: 600;
      margin-bottom: 8px;
    }
    .user-info-text {
      font-size: 14px;
      line-height: 2;
      i {
        margin-right: 8px;
        vertical-align: middle;
      }
      span {
        vertical-align: middle;
      }
    }
  }
  .user-avatar {
    .user-avatar-png {
      display: block;
      width: 110px;
      height: 110px;
      margin: 0 auto 20px;
      box-shadow: 2px 0 8px 0 rgba(29, 35, 41, 0.05);
      border-radius: 50%;
      background-color: #000;
      object-fit: contain;
    }
  }
  .user-name {
    font-size: 24px;
    font-weight: 500;
    text-align: center;
    line-height: 2;
  }
  .user-status {
    margin-top: 8px;
    font-size: 16px;
    font-weight: 400;
    text-align: center;
  }
}
@media screen and (max-width: 720px) {
}
</style>
