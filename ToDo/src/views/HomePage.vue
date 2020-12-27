<template>
    <div class="HomePage">
        <tasks-list />
    </div>
</template>

<script>
import TasksList from "@/components/HomePage/TasksList.vue"
export default {
    name: "HomePage",
    components: {
        TasksList
    }
}
</script>