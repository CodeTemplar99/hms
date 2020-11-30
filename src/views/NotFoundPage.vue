<template>
  <div>
    <!-- Header -->
    <div class="header bg-gradient-success py-7 py-lg-8 pt-lg-9">
      <b-container>
        <div class="header-body text-center mb-7">
          <b-row class="justify-content-center">
            <b-col xl="5" lg="6" md="6" class="px-5">
              <h1 class="text-white">Ooops!</h1>
              <p class="text-lead text-white">Page not found. Don't worry though, we have plenty of other pages to explore</p>

              <router-link to="/dashboard" class="font-weight-bold text-white mt-5">Back to dashboard</router-link>
            </b-col>
          </b-row>
        </div>
      </b-container>
    </div>
    </div>
</template>

<script>

export default {
  name: 'not-found'
};
</script>
