<template>
  <block
    id="Room"
    class=" bg-accent"
    :title="blockTitle"
  >
    <rooms-list />
  </block>
</template>
<script>
import Block from './Block.vue'
import RoomsList from './RoomsList.vue'

export default {
  name: 'RoomsBlock',
  components: { Block, RoomsList },
  data () {
    const blockTitle = {
      zh: '房間介紹',
      en: 'ROOMS'
    }
    return {
      blockTitle
    }
  }
}
</script>
