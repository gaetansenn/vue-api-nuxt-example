<template>
  {{ users }}
</template>

<script setup lang="ts">
// const { data: users } = await useFetch('https://64cbdfbd2eafdcdc85196e4c.mockapi.io/users')

// console.log('data useFetch', users.value)



// Test of composable useFetchModel
const { useFetch } = useFetchModel()

const { data: users } = await useFetch.get('https://64cbdfbd2eafdcdc85196e4c.mockapi.io/users')

console.log('data useFetchModel', users.value)




// Composable of composable test
// const { get } = useApiUsers()

// const users = await get()

// console.log(users.data.value)
</script>
