<template>
  <footer class="footer px-4">
    <b-row align-v="center" class="justify-content-lg-end">
      <b-col lg="12">
        <div class="copyright text-center text-lg-right text-muted">
          © {{year}} <span class="font-weight-bold ml-1">UNN</span>
        </div>
      </b-col>
    </b-row>
  </footer>
</template>
<script>
  export default {
    data() {
      return {
        year: new Date().getFullYear()
      };
    }
  };
</script>
<style></style>
