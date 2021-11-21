<template>
  <div>
      <v-card height="80vh" width="80vw">
        <v-subheader   style="background-color:#f1f1f1;" >
          <v-row>
            <v-btn text icon><v-icon size="30">mdi-arrow-left</v-icon></v-btn>
          </v-row>
      </v-subheader>
      <div class="mt-3" style="overflow:hidden;overflow-y:scroll;height:68vh">

        <div class="ma-8">
            
           <v-simple-table fixed-header >
    
      <thead>
        <tr>
          <th class="text-left">
            Device
          </th>
          <th class="text-left">
            Request
          </th>
          <th class="text-left">
            Sender
          </th>
          <th class="text-left">
            Response
          </th>
          <th class="text-left">
            Timestamp
          </th>
          
         
        </tr>
      </thead>
      <tbody>

        <tr
          v-for="logs in logs"
          :key="logs.id"
        >
          
          <td>{{ logs.device }}</td>
          <td>{{ logs.request }}</td>
          <td>{{ logs.sender }}</td>
          <td>{{ logs.response }}</td>
          <td>{{ logs.timestamp }}</td>
          
        </tr>
      </tbody>
   
  </v-simple-table>
  
          </div>
      </div>
      </v-card>
  </div>
</template>

<script>
import logsData from "../Testdata/logs.json"
export default {
data: () => ({
    logs: logsData
})
}
</script>

<style>

</style>