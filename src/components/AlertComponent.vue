<script setup>
// defineProps(['type' , 'msg'])
defineProps({
    type: {
        type:String,
        default: 'info'
    },
    msg: {
        type: String,
        default: "This is a default alert"
    }
})

const alertType = (type) => {
    const colors = {
        success: 'bg-green-100 text-green-800',
        danger: 'bg-red-100 text-red-800',
        warning: 'bg-yellow-100 text-yellow-800',
        info: 'bg-blue-100 text-blue-800'
    }
    return colors[type] || colors['info']
}

</script>
<template>
    <div class="p-4 mb-4 text-sm rounded-lg" :class = "alertType(type)" role="alert">
  <span class="font-medium">{{ msg }}</span> 
</div>
</template>

<style scoped>
button {
    padding: 10px;
    background-color: #007bff;
    color: #fff;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}
</style>
