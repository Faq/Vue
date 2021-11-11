<template>
  <button class="button" @click="onClick">{{ text }}</button>
  <div class="divider"/>
</template>

<script lang="ts">
import {Options, Vue} from 'vue-class-component';
import "./button.scss";

@Options({
  props: {
    text: {
      type: String,
      required: true,
    },
    onClick: Function,
  },
})
export default class Button extends Vue {
  text!: string
}
</script>
