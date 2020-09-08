<template>
  <header class="general-header-wrap">
    <div class="general-header block-wrap">
      <a href="/" class="logo-group">
        <h1 class="logo-title">Cozy House</h1>
        <span class="logo-description">Shelter for pets in Boston</span>
      </a>
      <nav class="header-menu">
        <a
          :href="`#${link.href}`"
          class="menu-item"
          v-for="(link, index) in menuItems"
          :key="`header-menu-item-${index}`"
        >
          {{ link.title }}
        </a>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data () {
    return {
      menuItems: [
        {
          title: 'About the shelter',
          href: '/about'
        },
        {
          title: 'Our pets',
          href: '/our-pets'
        },
        {
          title: 'To help the shelter',
          href: '/help-shelter'
        },
        {
          title: 'Contacts',
          href: '/contacts'
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
  @import "header";
</style>
