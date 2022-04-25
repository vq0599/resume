<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import Icon from './components/Icon.vue'
import Module from './components/Module.vue'
import Companies from './components/Companies.vue'
</script>

<template>
  <header>
    <strong>宙斯同学</strong>
    <span>求职意向：路由器工程师</span>
  </header>
  <div class="vq-profile">
    <span><Icon name="vq--gender" />男</span>
    <span><Icon name="vq--age" />28</span>
    <span><Icon name="vq--location" />深圳</span>
    <span><Icon name="vq--university" />新东方烹饪大学</span>
    <span><Icon name="vq--profession" />卤鹅专业</span>
    <span><Icon name="vq--telphone" />185xxxxxxxx</span>
    <span><Icon name="vq--mail" />xxxx@gmail.com</span>
  </div>
  <Companies />
  <Module title="技能介绍">
    <ul class="ul-box">
      <li>原生JavaScript基础好，TypeScript也有所掌握</li>
      <li>对React和Vue技术栈都有过比较深入的学习和实践，且具备带领相关的大型前端项目的经验</li>
      <li>了解NodeJS相关技术，能够基于主流Web框架完成一般项目的开发</li>
    </ul>
  </Module>
  <Module title="自我评价">
    <ul class="ul-box">
      <li>重视规则，厌烦黑盒事物，对团队协作效率比较关注</li>
      <li>设计公司出身，更加重视产品交互与用户体验</li>
      <li>不拘泥于具体技术栈，需要什么就能拾起什么</li>
    </ul>
  </Module>
</template>

<style lang="scss" scoped>
.ul-box {
  li {
    margin-top: 6px;
  }
}
:deep(.module-title) {
  margin-top: 40px;
}
</style>
