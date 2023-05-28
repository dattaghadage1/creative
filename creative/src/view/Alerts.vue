<template>
  <div class="container">
    <h3 class="h4 text-success font-weight-bold mb-4 mt-5">Alerts</h3>
    <base-alert icon="ni ni-like-2" dismissible type="success">
      <!-- <div slot="text">
        <strong>Success!</strong> This is a success alert—check it out!
      </div> -->
      <template v-slot:text>
        <strong>Success!</strong> This is a success alert—check it out!
      </template>
    </base-alert>
    <div class="col-lg-4 col-md-6">
      <BaseToast class="bg-warning">
        <template v-slot:header-content>
          <img src="img/tim.png" class="rounded mr-2" alt="logo" />
          <strong class="mr-auto text-white">Creative Tim</strong>
          <small class="text-white">Active</small>
        </template>
        <!-- <div slot="text" class="text-white">
          Heads up, toasts will stack automatically
        </div> -->
      </BaseToast>
    </div>

  </div>
</template>
<script>
import BaseAlert from '../components/BaseAlert.vue';
import BaseToast from "../components/BaseToast.vue"
export default {
  name: "alert-compo",
  components: {
    BaseAlert,
    BaseToast
  },
};
</script>
<style></style>
