<script lang="ts" setup>
const option = reactive({ title: 'title', description: 'desc' });
</script>

<template>
  <div class="container">
    <div>
      <Logo
        :option1="option"
        :option2="option"
        :option3="option"
        :option4="option"
      />
    </div>
  </div>
</template>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
