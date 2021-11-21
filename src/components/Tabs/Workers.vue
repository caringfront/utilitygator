<template>
  <div>
    <v-list flat>
      <v-list-item-group
        v-for="workers in workers" :key="workers.id"
        color="primary"
      >
       <router-link :to="workers.link" custom v-slot="{ navigate }">
        <v-list-item
        @click="navigate" role="link"
          link
        >
          <v-list-item-icon>
            <v-avatar dark class="orange white--text">{{workers.avatar}}</v-avatar>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>{{workers.name}}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
       </router-link>
      </v-list-item-group>
    </v-list>
  </div>
</template>

<script>
import workersData from "../../Testdata/workers.json"
  export default {
    data: () => ({
        workers: workersData,
    }),
  }
</script>

<style scoped>

</style>