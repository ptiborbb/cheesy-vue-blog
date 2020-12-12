<template>
  <div class="row">
    <div class="col-md-3"></div>
    <div class="col-md-6">
      <li v-for="item in articles" :key="item.message">
        <h3>
          <a href="">{{ item.title }}</a>
        </h3>
        <p>
          <em>Posted: {{ item.date }}</em>
        </p>
        <p>{{ item.body }}</p>
        <hr />
      </li>
    </div>
    <div class="col-md-9"></div>
  </div>
</template>

<script>
export default {
  name: "Articles",
  props: {
    articles: Array,
  },
};
</script>