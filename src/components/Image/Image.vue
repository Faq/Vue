<template>
  <img :src=image alt="Some image"> />
  <div class="divider"/>
</template>

<script lang="ts">
import {Options, Vue} from 'vue-class-component';
import "./image.scss";

@Options({
  props: {
    image: {
      type: String,
      required: true,
    },
    onClick: Function,
  },
})
export default class Image extends Vue {
  image!: string
}
</script>

<style scoped>
img {
  width: 280px;
  height: 120px;
}
</style>
