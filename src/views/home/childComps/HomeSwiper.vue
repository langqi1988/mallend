<template>
  <Swiper v-if="banners.length > 0">
    <Slide
      v-for="(item,index) in banners"
      :key="index"
    >
      <a :href="item.link">
        <img
          class="swiper-img"
          :src="item.image"
          alt=""
        >
      </a>
    </Slide>
  </Swiper>
</template>
<script>
import { Swiper, Slide } from "vue-swiper-component";
export default {
  props: {
    banners: {
      type: Array,
      default() {
        return [];
      },
    },
  },
  components: { Swiper, Slide },
  data() {
    return {};
  },
  mounted() {},
  methods: {},
};
</script>

<style scoped>
.swiper-img{
  width: 100%;
}
</style>