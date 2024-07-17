<!-- <template>
    <h2>
        First Page Component
    </h2>
    <input v-model="model" />
    <div>userName in Child is : {{ model }}</div>
</template>

<script setup lang="ts">
    const model:any = defineModel()
</script> -->


<!-- with arguments from below -->
<template>
    <h2>
        First Page Component
    </h2>
    <div>
        <input v-model="firstName" />
        <span>firstName in child  is : {{firstName}}</span>
    </div>
    <div>
        <input v-model="lastName" />
        <span>lastName in child is : {{ lastName }}</span>
    </div>
</template>
<script setup lang="ts">
    const firstName = defineModel('firstName')
    const lastName = defineModel('lastName')
</script>
<!-- with arguments upto above -->