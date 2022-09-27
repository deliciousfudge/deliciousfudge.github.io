<script>
  export default {
    props: ['entry']
  }
</script>

<template>
  <div>
    <h3>{{entry.provider}}</h3>
    <p>{{entry.dateFrom}} - {{entry.dateTo}}</p>
    <ul>
      <li v-for="descriptor in entry.descriptors">{{descriptor.name}}</li>
    </ul>
    </div>
</template>
