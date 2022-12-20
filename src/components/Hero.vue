<template>
  <div class="container py-5">
    <div class="row align-items-center text-center">
      <div :class="'col-md-6 p-5 ' + (orderNum ? 'order-' + orderNum : '')">
        <h1 class="display-6 fw-bold">{{ title }}</h1>
        <p class="lead" v-html="text"></p>
        <a :href="buttonUrl" class="btn btn-outline-dark" v-if="buttonUrl">{{
          buttonText
        }}</a>
      </div>
      <div class="col-md-6">
        <img
          :src="image"
          class="img-fluid rounded-3 shadow-lg"
          alt="Hero - Image"
          loading="lazy"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Components - Hero",
  props: {
    image: {
      default: null,
      type: String,
    },
    title: {
      default: null,
      type: String,
    },
    text: {
      default: null,
      type: String,
    },
    orderNum: {
      default: null,
      type: Number,
    },
    buttonText: {
      default: "Click here",
      type: String,
    },
    buttonUrl: {
      default: null,
      type: String,
    },
  },
};
</script>
