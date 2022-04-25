<template>
  <section class="module">
    <div class="module-title">
      <span>{{ title }}</span>
    </div>
    <slot />
  </section>
</template>

<script>
export default {
  props: {
    title: String
  }
}
</script>

<style lang="scss" scoped>
.module {
  &-title {
    border-bottom: 1px solid #572734;
    margin-bottom: 15px;
    span {
      display: block;
      padding: 8px 0;
      width: 160px;
      color: #FFF;
      text-align: center;
      background: #572734;
      font-size: 18px;
      font-weight: 600;
      letter-spacing: 5px;
    }
  }
}
</style>