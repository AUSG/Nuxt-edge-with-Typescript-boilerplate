<template>
  <a class="menu">
    <div class="title">{{ title }}</div>
    <hr/>
    <div class="subtitle">{{ subtitle }}</div>
  </a>
</template>

<script lang="ts">
import { Vue, Component, Prop } from 'nuxt-property-decorator'

@Component
export default class TopBarMenuComponent extends Vue {
  @Prop({ required: true })
  title: string | undefined
  @Prop({ required: true })
  subtitle: string | undefined
}
</script>

<style scoped>
hr {
  border: solid 3px white;
}

.menu {
  margin-right: 2em;
}

.title {
  width: 35px;
  height: 17px;
  font-family: Arial;
  font-size: 15px;
  font-weight: bold;
  font-style: normal;
  font-stretch: normal;
  line-height: normal;
  letter-spacing: normal;
  color: #ffffff;
}

.subtitle {
  margin-top: 1.5em;
  width: 152px;
  height: 17px;
  font-family: Arial;
  font-size: 15px;
  font-weight: bold;
  font-style: normal;
  font-stretch: normal;
  line-height: normal;
  letter-spacing: normal;
  color: #ffffff;
}

a {
  text-decoration: none;
}
</style>
