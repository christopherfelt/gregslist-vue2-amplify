<template>
  <b-container style="height:75vh" class="">
      <b-row class="h-100 d-flex align-items-center">
          <b-col>
              <Card title="Cars" description="Click to See Cars" redirectUrl="/cars" />
          </b-col>
          <b-col>
              <Card title="Houses" description="Click to See Houses" />
          </b-col>
          <b-col>
              <Card title="Jobs" description="Click to See Jobs" />
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