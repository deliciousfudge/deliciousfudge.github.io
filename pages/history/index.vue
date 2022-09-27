<script>
  import history from '../../data/history.json';
  import WorkEntry from '../../components/WorkEntry.vue'

  export default {
    data() {
        return {
            work: history.work,
            education: history.education
        };
    },
    components: { WorkEntry }
}
</script>

<template>
  <main>
    <h1>History</h1>
    <h2>Work</h2>
    <div v-for="entry in work">
      <WorkEntry v-bind:entry=entry />
    </div>
    <h2>Education</h2>
    <div v-for="entry in education" >
      <EducationEntry v-bind:entry=entry />
    </div>
  </main>
</template>
