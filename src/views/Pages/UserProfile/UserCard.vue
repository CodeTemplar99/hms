<template>
  <b-card no-body class="card-profile" alt="Image placeholder" img-top>
    <b-row class="justify-content-center">
      <b-col lg="8" class="order-lg-2">
        <div class="card-profile-image">
          <a href="#">
            <b-img src="img/theme/team-4.jpg" rounded="circle" />
          </a>
        </div>
      </b-col>
    </b-row>

    <b-card-header class="text-center border-0 pt-8 pt-md-4 pb-0 pb-md-4">
      <div class="d-flex justify-content-between">
        <a href="#" class="btn btn-sm btn-info mr-4 invisible"></a>
        <a
          href="#"
          class="btn btn-sm btn-outline-dark float-right"
          @click="printProfile"
          >print profile</a
        >
      </div>
    </b-card-header>

    <b-card-body class="pt-0">
      <b-row>
        <b-col>
          <div class="card-profile-stats d-flex justify-content-center mt-md-6">
            <div>
              <span class="heading">200</span>
              <span class="description">Level</span>
            </div>
            <div>
              <span class="heading">2019/2020</span>
              <span class="description">Session</span>
            </div>
            <div>
              <span class="heading">Current hall</span>
              <span class="description">Aja Nwachukwu</span>
            </div>
          </div>
        </b-col>
      </b-row>
      <div class="text-center">
        <h5 class="h1">Kelechi Pyragle</h5>
        <div class="h3 mt-4">Computer Science, Physical Science</div>
        <div>
          <i class="ni education_hat mr-2"></i>University of Computer Science
        </div>
        <hr class="my-4" />
        <p>
          --profile details gotten from student portal ---Please refer to
          student portal for changes
        </p>
        <!-- <a href="#">Show more</a> -->
      </div>
    </b-card-body>
  </b-card>
</template>
<script>
export default {
  methods: {
    printProfile: function () {
      window.print();
    },
  },
};
</script>
<style>
@media screen and (max-width: 320px) {
  .card-profile-stats {
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
}
</style>
