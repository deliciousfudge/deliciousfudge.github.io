<script>
  export default {
    props: ['entry']
  }
</script>

<template>
  <div>
    <h3>{{entry.employer}}</h3>
    <p>{{entry.position}}</p>
    <p>{{entry.dateFrom}} - {{entry.dateTo}}</p>
    <ul>
      <li v-for="descriptor in entry.descriptors">{{descriptor}}</li>
    </ul>
  </div>
</template>
