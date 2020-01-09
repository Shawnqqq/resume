<template>
  <div class="home-page">
    <div class="user-section">
      <el-row :gutter="40">
        <el-col :lg="12">
          <div class="grid-content">
            <h3 class="sub-title">能力简介</h3>
            <ul class="user-power">
              <li>
                1、熟练使用
                HTML、CSS、JavaScript，能高效率还原设计稿、动画及业务逻辑交互。
              </li>
              <li>
                2、掌握使用前端框架以及各种插件，jQuery、 Vue、Element Ui 、Ant
                等。
              </li>
              <li>3、熟悉移动端开发，能兼容移动版H5、微信小程序移动版产品。</li>
              <li>4、熟悉前端工程化搭建、webpack、Glup、Git。</li>
              <li>
                5、熟悉后端 Node.js，能操作
                Express、Koa能快速启动项目、独立敏捷开发，并有丰富的项目实战经验。
              </li>
              <li>
                6、工作中踏踏实实的敲代码，善于解决问题，对技术有深厚兴趣，爱折腾。
              </li>
            </ul>
          </div>
        </el-col>
        <el-col :lg="12">
          <div class="grid-content">
            <h3 class="sub-title">技能清单</h3>
            <ul class="user-power">
              <li>
                Web开发：
                <el-tag size="small">HTML</el-tag>
                <el-tag size="small">CSS</el-tag>
                <el-tag size="small" type="danger">JavaScript</el-tag>
              </li>
              <li>
                Web框架：
                <el-tag size="small" type="danger">Node.js</el-tag>
                <el-tag size="small" type="danger">Express</el-tag>
                <el-tag size="small">Koa2</el-tag>
              </li>
              <li>
                前端框架：
                <el-tag size="small">jQuery</el-tag>
                <el-tag size="small" type="danger">Vue</el-tag>
                <el-tag size="small">Element UI</el-tag>
                <el-tag size="small">Ant UI</el-tag>
                <el-tag size="small">Vant UI</el-tag>
                <el-tag size="small" type="danger">微信小程序</el-tag>
              </li>
              <li>
                前端工具：
                <el-tag size="small">Webpack</el-tag>
                <el-tag size="small">Gulp</el-tag>
                <el-tag size="small">Vue CLI3</el-tag>
              </li>
              <li>
                数据存储：
                <el-tag size="small">MySQL</el-tag>
                <el-tag size="small">XAMPP</el-tag>
              </li>
              <li>
                版本管理：
                <el-tag size="small">Git</el-tag>
                <el-tag size="small">Github</el-tag>
              </li>
            </ul>
          </div>
        </el-col>
      </el-row>
    </div>
    <div class="work-section">
      <h3 class="sub-title">项目经验</h3>
      <div class="block">
        <el-timeline>
          <el-timeline-item
            type="success"
            timestamp="2019.5～ 2019.12 扎克斯科技 - 前端研发，负责项目后台和专题页展示型网页开发。"
            placement="top"
          >
            <el-row :gutter="40" class="mobile-row">
              <el-col :lg="12">
                <div class="grid-content">
                  <el-card>
                    <h4 class="card-title">
                      糖果屋（ 个人项目 ）
                    </h4>
                    <p class="card-text">
                      <span>项目描述：</span>用Node.js 环境中使用 Express
                      快速搭建服务框架，七牛云管理图片，Vue
                      Cli搭建后台管理页，微信小程序展示产品功能的一个商用微信小程序；类似淘宝与美团的商用交易系统，用户能看到通过后台配置的展示的内容，并选择商品下单到服务器上；并且还具备商家查看订单、配送订单的操作能力。
                    </p>
                    <p class="card-text">
                      <span>项目成就：</span
                      >对微信小程序开发中的各种API有比较全面的了解；同时，对于后端的
                      MVC 操作模式以及 Knex
                      的数据操作方法能全面的运用，根据业务逻辑自行构思原型图，创建mysql表格；极大提升我对项目业务的逻辑思维能力和微信小程序框架的深度开发。
                    </p>
                  </el-card>
                </div>
              </el-col>
              <el-col :lg="12">
                <div class="grid-content">
                  <el-card>
                    <h4 class="card-title">
                      信息发布系统（ 极客学院教研项目 ）
                    </h4>
                    <p class="card-text">
                      <span>项目描述：</span
                      >极客学院的信息发布系统，通过后台配置的内容在前台中进行展示，支撑企业的信息发布和信息管理，运营人员会定期发布极客学院的新的动态及技术内容帮助大家及时的掌握前沿技术动态，更好的学习规划。为此需要一套信息管理发布系统来方便对他的内容进行发布、修改、删帖和分类等。
                    </p>
                    <p class="card-text">
                      <span>项目成就：</span>通过本项目，对 Node.js API
                      有更深入的了解，接下来可以完成 80% 的内容 API 设计。同时对
                      Vue 、Vue-router 及 Element-Ui 有实战行的应用。Vue-CLI
                      中的公共模板管理。在技术点上还涉及到 Vue-CLI
                      和其他后端框架 Express 的融合。
                    </p>
                  </el-card>
                </div>
              </el-col>
              <el-col :lg="12">
                <div class="grid-content">
                  <el-card>
                    <h4 class="card-title">
                      销售管理系统（ 扎克斯外包项目）
                    </h4>
                    <p class="card-text">
                      <span>项目描述：</span
                      >企业吸引更多的消费者，和广告公司合作做出各类精良的营销落地页，并在各个社交、媒体平台中进行投放。为了更好地获取广告信息，指导投放营销，需要一套承接这类营销落地页收集用户的购买行为信息，并进行跟踪、统计、反馈的管理系统。
                    </p>
                    <p class="card-text">
                      <span>项目成就：</span>通过本项目，在 Node.js 环境中使用
                      Express 快速搭建服务框架，并熟悉简单的 MySQL
                      数据库操作，可以完成数据的增删改查以及连表查询数据。同时，我们还对后端中
                      MVC
                      有深入的了解和实际的运用，懂得了在一个项目中数据是如何从数据库渲染到页面，页面是如何与服务端进行交互从而影响数据的变化。
                    </p>
                  </el-card>
                </div>
              </el-col>
              <el-col :lg="12">
                <div class="grid-content">
                  <el-card>
                    <h4 class="card-title">
                      目标与成就管理系统（ 扎克斯外包项目 ）
                    </h4>
                    <p class="card-text">
                      <span>项目描述：</span>OKR
                      为探月学院内部研发的目标管理的系统，能够将目标管理自上而下贯穿到基层。通过要设定一个“目标”（Objective），然后，设定若干可以量化的“关键结果”（Key
                      Results），用来帮助实现目标。
                    </p>
                    <p class="card-text">
                      <span>项目成就：</span>通过本项目首先对 OKR
                      有一个初步的认识，之前没有丁点概念，也熟悉企业的管理机制。在项目中使用
                      Koa2 来构建简易的 API，对 Nodejs API
                      的生产有更熟悉的运用，同时对小程序开发有一定的了解，能够完成负责业务场景下的小程序研发工作。
                    </p>
                  </el-card>
                </div>
              </el-col>
              <el-col :lg="12">
                <div class="grid-content">
                  <el-card>
                    <h4 class="card-title">营销活动页开发（扎克斯外包项目）</h4>
                    <p class="card-text">
                      <span>项目描述：</span
                      >完成营销、活动、专题项目的样式和交互，服务过的公司有：Toppro、极客学院、高通等等，主要使用
                      HTML、CSS、JavaScript 完成页面样式和交互开发。
                    </p>
                    <p class="card-text">
                      <span>项目成就：</span
                      >通过多个项目的训练，对设计稿的还原度以及交付效率有质的提升，能给高效、快速地
                      1 : 1还原设计文件，同时 JavaScript
                      的语感提升为之后的多页面项目研发打下基础。
                    </p>
                  </el-card>
                </div>
              </el-col>
            </el-row>
          </el-timeline-item>
        </el-timeline>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  components: {}
};
</script>

<style type="text/css" lang="less" scoped>
@media screen and (max-width: 720px) {
  .mobile-row {
    margin-left: -30px !important;
    margin-right: -30px !important;
  }
}
.home-page {
  padding: 40px;

  .sub-title {
    font-size: 18px;
    margin-bottom: 16px;
  }

  .card-title {
    font-size: 16px;
    margin-bottom: 8px;
  }

  .card-text {
    font-size: 14px;
    color: #666;
    margin: 8px 0;
    span {
      font-size: 14px;
      color: #333;
      font-weight: 600;
      display: block;
    }
  }

  .user-power {
    list-style: none;
  }

  .grid-content {
    margin-bottom: 20px;
    font-size: 14px;
    line-height: 2;
  }

  .el-tag {
    margin-right: 8px;
  }
}
</style>
