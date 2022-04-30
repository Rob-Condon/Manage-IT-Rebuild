<template class="MainAPP">
  <MainBar/>
  <router-view/>
</template>
<script>
import { mergeGlobalConfig } from 'vuestic-ui'
import MainBar from '@/components/navagation/MainBar.vue'
export default {
  components: {MainBar},
  setup () {
    mergeGlobalConfig({
      colors: {
        primary: '#293F14',
        secondary: '#386C0B',
        link: '#E1CBF6'
      }
    })
  }
}

</script>
<style>
.MainAPP {
  overflow-x: hidden;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

a:hover {
  color: var(--va-link);
}

a {
  color: var(--va-background);
}

.va-navbar__item {
  align-self: center;
}

.primary {
  color: var(--va-primary);
}

.secondary {
  color: var(--va-secondary);
}

.link {
  color: var(--va-link);
}

.text-size-tiny {
  font-size: .625rem;
}

.text-size-small {
  font-size: 0.85rem;
}

.text-size-normal {
  font-size: 1.2rem;
}

.mw-900 {
  max-width: 900px
}
</style>
