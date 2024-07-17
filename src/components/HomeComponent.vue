<!-- <template>
    <h1>
        Home Component
    </h1>
    <div>userName in Parent is : {{ userName }}</div>
    <FirstPage v-model="userName"></FirstPage>
</template>

<script setup lang="ts">
    import FirstPage from "./FirstPageComponent.vue"
    import { ref } from "vue"
    import type { Ref } from "vue"

    const userName: Ref<string> = ref("Ahamad")
</script> -->


<!-- with arguments from below -->
<template>
    <h1> Home Component </h1>
    <div>
        FirstName is : {{ firstName }}
    </div>
    <div>
        LastName is : {{ lastName }}
    </div>
    <FirstPage v-model:firstName="firstName" v-model:lastName="lastName"></FirstPage>
</template>
<script setup lang="ts">
    import FirstPage from "./FirstPageComponent.vue"
    import { ref } from 'vue'
    import type { Ref } from "vue"

    const firstName: Ref<string> = ref('Ahamad')
    const lastName: Ref<string> = ref('Shaik')
</script>
<!-- with arguments upto above -->