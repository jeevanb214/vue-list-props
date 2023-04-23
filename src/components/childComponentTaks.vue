<template>
    <ul>
        <li>
            <div>{{ task.name }} --- {{ index }}</div>
            <small>{{ task.dueDate }} @ {{ task.dueTime }}</small>
           <!--  <button @click="deleteTask(index)">X</button> -->
        </li>
    </ul>
</template>



<script>

export default ({
    props: ['task', 'index'],

/*     methods: {
        deleteTask(index) {
            console.log(index)
            this.tasks.splice(index, 1);
            console.log(this.tasks);
        }
    }, */
})

</script>



<style ></style>