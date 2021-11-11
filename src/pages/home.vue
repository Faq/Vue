<template>
  <h1>{{ msg }}</h1>
  <Button text="All"/>
  <Button text="C#"/>
  <Button text="C++"/>
  <Button text="Delphi"/>
  <Button text="PHP"/>
  <Button text="Ruby"/>
</template>

<script lang="ts">
import {Options, Vue} from 'vue-class-component';
import Button from "@/components/Button/Button.vue";
import Image from "@/components/Image/Image.vue";

@Options({
  props: {
    msg: String
  },
  components: {
    Button,
    Image,
  },
  methods: {}
})
export default class HelloWorld extends Vue {
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.button {
  margin: 40px 0 0;
}

</style>
