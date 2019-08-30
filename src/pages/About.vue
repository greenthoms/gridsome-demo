<template>
  <Layout>
    <Card />
    <h1>About us</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Error doloremque omnis animi, eligendi magni a voluptatum, vitae, consequuntur rerum illum odit fugit assumenda rem dolores inventore iste reprehenderit maxime! Iusto.</p>
    <b-alert show>Default Alert</b-alert>
    <b-alert variant="success" show>Success Alert</b-alert>
  </Layout>
</template>

<script>
import Card from '~/components/Card.vue'

export default {
  metaInfo: {
    title: 'Test'
  },
  components: {
    Card
  }
}
</script>
