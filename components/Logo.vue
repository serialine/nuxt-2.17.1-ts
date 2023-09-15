<script lang="ts" setup>
interface Option1 {
  title?: string;
  description?: string;
}
interface Option2 {
  title: string;
  description?: string;
}

defineProps<{
  option1: Option1;
  option2: Option2;
  option3: Required<Option1>;
  option4: Partial<Option2>;
}>();
</script>

<template>
  <div>
    {{ option1.title }}
    <!-- Property 'title' does not exist on type 'unknown'.ts(2339) -->
    {{ option2.title }}
    {{ option3.title }}
    {{ option4.title }}
    <!-- Property 'title' does not exist on type 'unknown'.ts(2339) -->
  </div>
</template>
