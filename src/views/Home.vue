<template>
  <assign-arrangers></assign-arrangers>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src
import AssignArrangers from "@/components/assign-arrangers.vue";

@Component({
  components: {
    HelloWorld,
    AssignArrangers
  }
})
export default class Home extends Vue {}
</script>
