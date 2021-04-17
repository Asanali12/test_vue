<template>
    <div>
        <ul>
            <ToDoItem
            v-for="todo in todos"
            :todo="todo"
            :key="todo.id"
            />
        </ul>
    </div>
</template>

<script>
import ToDoItem from "@/components/ToDoItem"
export default{
    props:["todos"],
    components:{
        ToDoItem
    }
}
</script>
