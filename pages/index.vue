<template>
  <div>
    <Nuxt />
    
    <pre>
      {{ $store.state.user }}
    </pre>

    <pre>
      {{ user }}
    </pre>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import { mapState } from 'vuex';

export default Vue.extend({
  name: 'IndexPage',

  computed: {
    ...mapState({
      user: state => state.user,
    })
  },
})
</script>
