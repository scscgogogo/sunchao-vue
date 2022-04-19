<template>
  <h3>{{ name }}</h3>
  <label for="tag-1">
    <input
      type="checkbox"
      id="tag-1"
      v-model="tags"
      value="千岛湖"
      @change="setName"
    />
    千岛湖
  </label>
  <label for="tag-2">
    <input type="checkbox" id="tag-2" v-model="tags" value="太湖" />
    太湖
  </label>
  <label for="tag-3">
    <input type="checkbox" id="tag-3" v-model="tags" value="云龙湖" />
    云龙湖
  </label>
  <span>→Tags:{{ tags }}</span>
</template>

<script>
export default {
  data() {
    return {
      name: 'SUNCHAO',
      tags: [],
    };
  },
};
</script>

<style>
@import './styles/app.css';
</style>
