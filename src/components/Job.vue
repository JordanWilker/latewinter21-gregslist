<template>
  <div class="col-4">
    <!-- NOTE the route contains both the name and an object to provide needed params -->
    <router-link :to="{name: 'JobsDetailsPage', params: {id: job._id}}" >
      <div class="card job">
        <div class="card-body">
          <h4 class="card-title">{{job.jobTitle}} | {{job.company}}</h4>
          <p class="card-text">{{job.rate}} | {{job.hours}}</p>
        </div>
      </div>
    </router-link>
  </div>
</template>

<script>
export default {
  name: 'job',
  props: {
    job: Object
  },
  setup() {
    return {}
  },
  components: {}
}
</script>

<style scoped>
.job:hover {
  transform: translateY(-5px);
  box-shadow: 1px 3px 5px rgb(94, 94, 94);
  cursor: pointer
}

.job {
  transition: all .2s;
  color: black
}
</style>
