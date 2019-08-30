<template>
  <Layout>
    <b-breadcrumb :items="items"></b-breadcrumb>
    <h1>Test</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Error doloremque omnis animi, eligendi magni a voluptatum, vitae, consequuntur rerum illum odit fugit assumenda rem dolores inventore iste reprehenderit maxime! Iusto.</p>
    <Alert />
    <b-container class="bv-example-row">
    <b-row>
        <b-col>1 of 3</b-col>
        <b-col>2 of 3</b-col>
        <b-col>3 of 3</b-col>
    </b-row>
    <b-table striped hover :items="items"></b-table>

    </b-container>
  </Layout>
</template>

<script>
import Alert from '~/components/Alert.vue'

export default {
  metaInfo: {
    title: 'About us'
  },
  components: {
    Alert
  },
  data() {
      return {
        items: [
          {
            text: 'Admin',
            href: '#'
          },
          {
            text: 'Manage',
            href: '#'
          },
          {
            text: 'Library',
            active: true
          }
        ]
      }
    }
}
</script>

<style scoped>
    .bv-example-row .row>.col:not(.header), .bv-example-row .row>[class^=col-] {
    padding-top: .75rem;
    padding-bottom: .75rem;
    background-color: rgba(86,61,124,.15);
    border: 1px solid rgba(86,61,124,.2);     
    }
</style>