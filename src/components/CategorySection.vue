<template>
  <div class="container">
    <section>{{ title }}</section>
  </div>
</template>

<script>
export default {
  name: "CategorySection",
  props: {
    title: String,
  },
};
</script>
