<template>
<layout>
  <b-container>
    <b-row v-for="type in types" :key="type">
      <b-col sm="6 form-group">
        <label :for="`type-${type}`">Type {{ type }}:</label>
        <b-form-input :id="`type-${type}`" :type="type"></b-form-input>
      </b-col>
    </b-row>
  </b-container>
  </layout>
</template>

<script>
  export default {
    metaInfo: {
    title: 'Form'
    },
    data() {
      return {
        types: [
          'text',
          'password',
          'email',
          'number',
          'url',
          'tel',
          'date',
          `time`,
          'range',
          'color',
          'textarea'
        ]
      }
    }
  }
</script>