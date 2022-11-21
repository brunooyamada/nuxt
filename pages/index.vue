<template>
  <div>
    <Nuxt />

    <VTooltip>
      <a>Sponsor me</a>

      <template #popper >
        Help me fund my Open Source work!
      </template>
    </VTooltip>
    
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

  data() {
    return {};
  },

  created() {
    console.log(this.$name('Jon Snow'));
  },

  mounted() {
    console.log(this.$dayjs().format());
  },

  computed: {
    ...mapState({
      user: state => state.user,
    })
  },
})
</script>
