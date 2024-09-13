<script lang="ts" setup>
const props = defineProps({
  path: String
});

function go() {
  const a = document.createElement("a");
  a.href = props.path == undefined ? "/" : props.path.toString();
  a.target = "_blank"
  a.click();
}
</script>

<template>
  <div class="button" v-on:click="go()">
    <a>
      <slot/>
    </a>
  </div>
</template>

<style scoped>
.button {
  width: 80%;
  height: 50px;
  margin: 1em auto;
  background-color: rgba(90, 57, 198, 0.7);
  cursor: pointer;
  border-radius: 50px;
  box-shadow: 5px 5px 10px rgba(0, 0, 0, 80%);
}

.button a {
  line-height: 50px;
  font-size: 20px;
  letter-spacing: 4px;
}
</style>