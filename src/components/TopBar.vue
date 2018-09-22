<template>
  <div class="topbar">
    <TopBarBrand class="topbar-brand"/>
    <div class="topbar-menubar">
      <TopBarMenu v-for="menu in menus" :key="menu.title" 
        :title="menu.title" :subtitle="menu.subtitle" :href="menu.href"/>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'nuxt-property-decorator'
import TopBarBrand from '~/components/TopBarBrand.vue'
import TopBarMenu from '~/components/TopBarMenu.vue'

@Component({
  components: {
    TopBarBrand,
    TopBarMenu,
  }
})
export default class TopBarComponent extends Vue {
  menus = [
    {
      title: 'AWS',
      subtitle: 'Amazon Web Service',
      href: '',
    }, {
      title: 'AWSKRUG',
      subtitle: 'AWS KoRea User Group',
      href: '',
    }, {
      title: 'AUSG',
      subtitle: 'Awskrug University Student Group',
      href: '',
    }
  ]
}
</script>

<style scoped>
.topbar {
  margin-top: 2em;
  display: flex;
}

.topbar-brand {
  flex: none;
}

.topbar-menubar {
  flex: 1 1 auto;
  display: flex;
  justify-content: flex-end;
  padding-right: 5em;
}

.topbar-menu {
  flex: 1 1 auto;
}
</style>
