<template>
  <q-page pdding>
    <childComponent 
    v-for="(task, index) in tasks" 
    :key="task.id" 
    :task="task"
    :index="index">{{ index }}</childComponent>
    <ul>

    </ul>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue'
import childComponentTaksVue from '../components/childComponentTaks.vue'

export default defineComponent({
  name: 'IndexPage',


  data() {
    return {
      tasks: [
        {
          id: 0,
          name: 'Go to shop',
          dueDate: '2019/05/1',
          dueTime: '18:30'
        },
        {
          id: 1,
          name: 'Get bananas',
          dueDate: '2019/05/1',
          dueTime: '14:00'
        },
        {
          id: 2,
          name: 'Get apples',
          dueDate: '2019/05/1',
          dueTime: '132.001'
        }
      ]
    }
  },

  components: {
    'childComponent': childComponentTaksVue
  }

})
</script>