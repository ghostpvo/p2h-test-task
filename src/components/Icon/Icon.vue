<template>
  <svg
    :class="iconId"
    class="icon"
    viewBox="0 0 100 100"
  >
    <!-- TODO '~' - не работал в обратных кавычках, временно поставил '/_nuxt/', надо сделать норм -->
    <use :xlink:href="getSprite(iconId)">
      {{ tittle }}
    </use>
  </svg>
</template>

<script>
export default {
  name: 'Icon',
  props: {
    icon: {
      type: String,
      default: ''
    },
    tittle: {
      type: String,
      default: ''
    },
    isActive: {
      type: Boolean,
      default: false
    }
  },
  computed: {
    iconId () {
      if (this.isActive) {
        return this.icon + '-active'
      } else {
        return this.icon
      }
    }
  },
  methods: {
    getSprite (type) {
      return require('../../assets/sprite/sprite.svg') + '#' + type
    }
  }
}
</script>
