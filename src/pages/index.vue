<template>
  <div class="main">
    <Intro/>
    <Ausg class="ausg"/>
  </div>
</template>

<script lang="ts">
import { Vue, Component, Prop } from 'nuxt-property-decorator'
import Intro from '~/components/Intro.vue'
import Ausg from '~/components/Ausg.vue'

@Component({
  components: {
    Intro,
    Ausg,
  }
})
export default class IndexPage extends Vue {

}
</script>

<style scoped>
.main {
  padding-top: 4em;
  padding-bottom: 25em;

  background-image: url('../static/img/path-3.png'), url('../static/img/oval.png');
  background-position: 0% 100%, 100% 95%;
  background-repeat: no-repeat;
  background-size: 1031.5px 741px, 326px 414px;
}

.ausg {
  margin-top: 15em;
}
</style>

