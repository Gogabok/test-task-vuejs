<template>
    <div class="TasksList">
        <tasks-input/>
        <task-item
            v-for="(task, index) in tasks"
            :key="`task-${index}`"
            :title="task.title"
        />
    </div>
</template>

<script>
import TaskItem from "@/shared-components/TaskItem"
export default {
    name: "TasksList",
    components: {
        TaskItem
    },
    data: () => ({
        tasks: [
            {
                title: "Сделать1"
            },
            {
                title: "Сделать2"
            },
            {
                title: "Сделать3"
            },
            {
                title: "Сделать4"
            },
        ]
    })
}
</script>