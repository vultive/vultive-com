<template>
  <section id="services" class="vultive-bg-muted">
    <div class="container py-5 text-center">
      <h1 class="fw-bold">Featured Services</h1>
      <div class="col-lg-6 mx-auto">
        <div
          class="row row-cols-1 row-cols-4 align-items-stretch g-4 py-2 text-light justify-content-center"
        >
          <template v-for="service in services" v-bind:key="service.name">
            <div class="col">
              <a :href="service.url" :aria-label="service.name">
                <img
                  :src="service.background"
                  width="96"
                  height="96"
                  class="img-fluid rounded vultive-service vultive-animations-fadeIn"
                  :alt="service.name"
                  loading="lazy"
                /></a
              >
            </div>
          </template>
        </div>
      </div>
    </div>
  </section>
  <section id="lss">
    <hero
      :image="require('@/assets/lss.jpg')"
      title="Live Streaming Service"
      text="our Live Streaming Service is a quick way to share your passion with
            the world! Whether you're a new streamer or an experienced gamer, we
            can help you broadcast your gameplay in high quality
            <span class='fw-bold'>for free.</span>"
    />
  </section>
  <section id="llp">
    <hero
      :image="require('@/assets/wip.jpg')"
      title="Language Learning Platform"
      text="our Language Learning Platform is the perfect tool for students,
            educators, and language enthusiasts. With extensive learning content
            with interactive exercises, we help you learn languages faster and
            more efficiently. All of our learning content is
            <span class='fw-bold'>free to use.</span>"
      orderNum="1"
    />
  </section>
</template>

<script>
import hero from "../components/Hero";
export default {
  name: "Views - Main",
  components: {
    hero,
  },
  data() {
    return {
      services: [
      {
          name: "Vultive LSS",
          background: require("@/assets/lss.favicon.jpg"),
          url: "https://lss.vultive.com",
        },
      ],
    };
  },
};
</script>
