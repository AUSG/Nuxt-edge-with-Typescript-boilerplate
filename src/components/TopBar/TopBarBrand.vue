<template>
  <a class="box" href="/">
    <span class="AWS">
      AWS한국사용자모임
    </span>
  </a>
</template>

<script lang="ts">
import { Vue, Component } from 'nuxt-property-decorator'

@Component
export default class TopBarBrandComponent extends Vue {
  
}
</script>

<style scoped>
.box {
  width: 300px;
  /* height: 0.1px; */
  /* border: solid 4px #ffffff; */
  border-top: solid 4px white;
}

.AWS {
  width: 172px;
  height: 26px;
  font-family: AppleSDGothicNeo;
  font-size: 20px;
  font-weight: 800;
  font-style: normal;
  font-stretch: normal;
  line-height: normal;
  letter-spacing: normal;
  color: #ffffff;
  margin: 0.5em;
  float: right;
}

.AWS .text-style-1 {
  font-family: Arial;
  font-size: 22px;
  font-weight: bold;
}
</style>
