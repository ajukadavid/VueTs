<template>

<div class="app">
 <p>
   {{jobs[0].location}}
 </p>
</div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';
import Job from './types/Job'


export default defineComponent({
  name: 'App',
  components: {},
  setup(){
    // const state = reactive({
    //   name: 'Link',
    //   age: 25 as string | number
    // })
    // state.name = 'shaun'
    // return {
    //   ...toRefs(state)
    // }

  //   const name = ref('Link')
  //   const age = ref<number | string>(12)


  //  return {
  //    name, age

  //  }

  const jobs = ref<Job[]>([ //this is an array of Job objects
      {
        title: 'Farm worker',
        location: 'lon lon ranch',
        salary: 30000,
        id: '1'
      },
      {
        title: 'quarryman',
        location: 'Death mountain',
        salary: 40000,
        id: '2'
      },
      {
        title: 'flute player',
        location: 'the lost woods',
        salary: 35000,
        id: '3'
      },
      {
        title: 'fisherman',
        location: 'lake hylia',
        salary: 21000,
        id: '4'
      },
      {
        title: 'prison guard',
        location: 'gerudo valley',
        salary: 32000,
        id: '1'
      }
  ])

  return {
    jobs
  }
  },


});
</script>

<style>

</style>
