<template>
  <card class="card-user">
    <!-- <div slot="image">
      <img src="@/assets/img/background.jpg" alt="...">
    </div> -->
    <br><br><br>
    <div>
      <div class="author">
        <img class="avatar border-white" src="@/assets/img/faces/rosadiaz.jpg" alt="...">
        <h4 class="title">Rosa Diaz
          <br>
          <a href="#">
            <small>San Diego, US - 56</small>
          </a>
        </h4>
      </div>
      <p class="description text-center">
       What kind of a woman Doesn't have an Ax
      </p>
    </div>
    <hr>
    <div class="text-center">
        <p-button type="success" round>Donate Now</p-button>&nbsp;
      <p-button type="info" round>Know More</p-button>
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
