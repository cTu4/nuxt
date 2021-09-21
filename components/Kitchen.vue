<template>
  <div>
    <div class="card">
      <div>
        {{ card.Name }}
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Component from 'vue-class-component'
import { Card } from '@/types/Card'

@Component({
  name: 'Kitchen',
  data () : any {
    return {
      test: 'aaaa'
    }
  }
})
export default class Kitchen extends Vue {
  test!: string
  card!: Card
  created (): void {
    console.log('aa')
    this.card = {
      Name: 'dish 1',
      Options: ['option1'],
      TimePlace: 1632242259,
      Table: 4,
      Comment: ['comment']
    }
  }
}
</script>

<style scoped>

</style>
