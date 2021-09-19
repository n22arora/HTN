<template>
  <card class="card-user">
    <!-- <div slot="image">
      <img src="@/assets/img/background.jpg" alt="...">
    </div> -->
    <br><br><br>
    <div>
      <div class="author">
        <img class="avatar border-white" src="@/assets/img/faces/jakeperalta.jpg" alt="...">
        <h4 class="title">Jake Peralta
          <br>
          <a href="#">
            <small>Brooklyn, US - 40</small>
          </a>
        </h4>
      </div>
      <p class="description text-center">
        Cool, cool, cool, cool, cool, cool....
      </p>
    </div>
    <hr>
    <div class="text-center">
      <!-- <button>Donate Now</button> -->
      <p-button type="success" round>Donate Now</p-button>&nbsp;
      <p-button type="info" round>Know More</p-button>
      <!-- <div class="row">
        <div v-for="(info, index) in details" :key="index" :class="getClasses(index)">
          <h5>{{info.title}}
            <br>
            <small>{{info.subTitle}}</small>
          </h5>
        </div>
      </div> -->
    </div>
  </card>
</template>
<script>
export default {
  data() {
    return {
      details: [
        {
          title: "12",
          subTitle: "Files"
        },
        {
          title: "2GB",
          subTitle: "Used"
        },
        {
          title: "24,6$",
          subTitle: "Spent"
        }
      ]
    };
  },
  methods: {
    getClasses(index) {
      var remainder = index % 3;
      if (remainder === 0) {
        return "col-lg-3 offset-lg-1";
      } else if (remainder === 2) {
        return "col-lg-4";
      } else {
        return "col-lg-3";
      }
    }
  }
};
</script>
<style>
</style>
