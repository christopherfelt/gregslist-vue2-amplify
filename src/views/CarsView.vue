<template>
  <b-container>
    <b-row>
      <b-col class="pt-4">
        <b-card-group columns>
          <Card v-for="car in cars" :key="car.id" :title="car.title" :description="car.description" cardStyle="" :imgSrc="car.imgSrc" />
        </b-card-group>
      </b-col>
    </b-row>
  </b-container>

</template>

<script>
import Card from "@/components/Card.vue"
export default {
  name: "CarsView",
  components: {
    Card
  },
  data(){
    return {
      cars: [
        {
          id: 1,
          title: "Car 1",
          description: "This is the first car",
          imgSrc: "https://placekitten.com/g/200/100?image=13"

        },
        {
          id: 2,
          title: "Car 2",
          description: "This is the second car",
          imgSrc: "https://placekitten.com/g/300/200?image=14"
        },
        {
          id: 1,
          title: "Car 1",
          description: "This is the first car",
          imgSrc: "https://placekitten.com/g/200/500?image=15"
        },
        {
          id: 2,
          title: "Car 2",
          description: "This is the second car"
        },
        {
          id: 1,
          title: "Car 1",
          description: "This is the first car"
        },
        {
          id: 2,
          title: "Car 2",
          description: "This is the second car"
        }
      ]
    }
  }
}
</script>

<style>

</style>