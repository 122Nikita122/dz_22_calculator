<template>
  <div >
    <VueClock />
  </div>
</template>

<script>

import VueClock from '../../node_modules/@dangvanthanh/vue-clock/src/VueClock';

export default {
    name: 'Watch',
    components: { VueClock }
}
</script>