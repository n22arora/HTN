<template>
<card class="card-user">
    <div slot="image">
      <img src="@/assets/img/background.jpg" alt="...">
    </div>
    <br><br><br>
    <div>
      <div class="author">
        <img class="avatar border-white" src="@/assets/img/faces/Melissa.jpg" alt="...">
        <h4 class="title">Amy Santiago
          <br>
          <a href="#">
            <small>Age: 38</small>
          </a>
        </h4>
      </div>
      <p class="description text-center">
        I am from New York, US
      </p>
    </div>
    <br>
    <div class="row">
      <div class="col" align="center"> 
        <h5 class="title"> Fun Facts</h5>
          I love reading terms and conditions of a contract<br>
          I don't like changing lanes without giving signal<br>
          I like to arrange things into tabs and put margins<br>
          I like the smell of an old binder<br>
      </div>
      <div class="col" align="center"> 
        <h5 class="title"> How I ended up here?</h5>
        I got shot in the leg then I coudn't serve for NYPD anymore. The money I saved up could help me with expenses for another 3 yrs. Then, I ended up being homeless after that money exhausted. 
      </div>
    </div>
    <hr>
    <div class="text-center">
      <p-button type="success" round>Donate Now</p-button>
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
