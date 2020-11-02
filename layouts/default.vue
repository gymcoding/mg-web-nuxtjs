<template>
  <nuxt />
  
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: '모두의발전기',
    }
  },
}
</script>
