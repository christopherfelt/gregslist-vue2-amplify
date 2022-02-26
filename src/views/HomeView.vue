<template>
  <b-container style="height:75vh" class="">
      <b-row class="h-100 d-flex align-items-center">
          <b-col>
              <Card title="Cars" description="Click to See Cars" redirectUrl="/cars" cardStyle="height:200px;"/>
          </b-col>
          <b-col>
              <Card title="Houses" description="Click to See Houses" cardStyle="height:200px;" />
          </b-col>
          <b-col>
              <Card title="Jobs" description="Click to See Jobs" cardStyle="height:200px;" />
          </b-col>
      </b-row>
  </b-container>
</template>

<script>
import Card from "@/components/Card.vue"

export default {
    name: "HomeView",
    components: {
        Card
    }

}
</script>

<style>

</style>