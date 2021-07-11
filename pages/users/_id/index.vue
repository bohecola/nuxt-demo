<template>
  <h1>A user -- ID: {{$route.params.id}}</h1>
</template>

<script>
export default {
  validate(data) {
    return /^\d+$/.test(data.params.id)
  }
}
</script>