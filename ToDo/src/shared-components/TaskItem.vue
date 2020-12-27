<template>
    <div class="TaskItem">
        <span class="TaskItem-title">{{ title }}</span>
        <div class="TaskItem-buttons-group">
            <button class="TaskItem-buttons-group__item">Удалить</button>
        </div>
    </div>
</template>

<script>
export default {
    name: "TaskItem",
    props: {
        title: {
            type: String,
            required: true
        }
    }
}
</script>

<style scoped>
    .TaskItem {
        border: 1px solid grey;
        border-radius: 4px;
        padding: 10px 15px;
        display: flex;
        align-items: center;
        cursor: pointer;
        user-select: none;
        margin: 5px 0px;
    }
    .TaskItem .TaskItem-title {
        font-size: 18px;
    }
    .TaskItem-buttons-group {
        margin-left: auto;
        display: flex;
        align-items: center;
    }
    .TaskItem-buttons-group__item {
        margin: 0px 5px;
    }
</style>