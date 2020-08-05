<template>
  <a class="articleItem"
     :href="getLink(item.id)">
    <img class="thumb"
         :src="item.thumb"
         v-show="hasThumb">
    <div class="title">{{ item.title }}</div>
  </a>
</template>
<script>

import ArticleItem from './ArticleItem.vue';

export default {
  name: 'Highlighted',
  extends: ArticleItem,
};
</script>

<style lang="scss" scoped>
.articleItem {
  padding: 12px;
  height: 180px;
  margin-bottom: 12px;
  background-color: lightcoral;
}

.thub {
  width: 160px;
  height: 160px
}

.title {
  font-size: 28px;
}
</style>
