<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import Module from './Module.vue'
</script>

<template>
  <Module title="职业经历">
    <div class="company">
      <div class="company-header">
        <span>小鸭科技（深圳）有限公司</span>
        <span>2019-07 — 至今</span>
      </div>
      <ul class="company-projects">
        <li>
          <h3>西瓜IDE（TypeScript、Node.js、Docker）</h3>
          <div>基于<a href="https://www.eclipse.org/che/">Eclipse Che</a>和VSCode的Web IDE项目。</div>
          <ul>
            <li>研究Che-Theia、VSCode等项目源码，实现了基于Che Server的容器调度的能力接入了VSCode IDE，取得了突破性的用户体验提升</li>
            <li>主导业务VSCode插件的开发，为Web IDE提供了在线Code Review、代码Clone等重要功能</li>
          </ul>
        </li>
        <li>
          <h3>苹果社区（Vue.js系列、TypeScript）</h3>
          <div>社区类项目，作为核心开发，除了日常的业务之外，我也在基础设施和研发提效上有所贡献。</div>
          <ul>
            <li>搭建UI组件库，TS源码+Gulp手写构建过程，大幅提高跨项目代码复用</li>
            <li>基于Vue CLI和<a href="https://github.com/tj/commander.js">Commander.js</a>封装了一套快速启动的CLI脚手架，助力活动运营页面研发提效</li>
          </ul>
        </li>
      </ul>
    </div>
    <div class="company">
      <div class="company-header">
        <span>北京橙子科技有限公司</span>
        <span>2017-06 — 2019-06</span>
      </div>
      <ul class="company-projects">
        <li>
          <h3>
            可视化建站系统（React系列、Next.js、Node.js）
            <a href="https://google.com" target="_blank">https://google.com</a>
          </h3>
          <div>
            一个集成了SPA编辑器、SSR同构渲染、小程序、H5页面等多个项目的大型重交互可视化建站系统，作为项目的前端owner，从0到1皆由我统筹规划。
          </div>
          <ul>
            <li>带领团队建立了Git工作流程、统一代码规范（ESlint）、倡导Code Review等</li>
            <li>设计项目架构，重交互的核心功能以React + Redux开发，用户访问端以Node.js + Next.js为基础同构渲染，以满足SEO和首屏快速渲染的强需求</li>
          </ul>
        </li>
        <li>
          <h3>
            柠檬招聘
            <a href="google.com" target="_blank">https://google.com/job</a>
          </h3>
          <div>标准的移动端React单页应用</div>
        </li>
      </ul>
    </div>
  </Module>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.company {
  &:nth-child(n+2) {
    margin-bottom: 30px;
  }
  &-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-size: 20px;
    margin-bottom: 10px;
    & > span:nth-child(1) {
      font-weight: bold;
    }
  }
  &-projects {
    h3 {
      font-weight: bold;
      font-size: 18px;
      margin-bottom: 10px;
    }
    & > li {
      margin-top: 15px;
    }
    ul {
      margin-top: 5px;
      padding-left: 20px;
      li {
        line-height: 1.8;
      }
    }
  }
}
</style>