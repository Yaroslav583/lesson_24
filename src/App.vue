<template>

  <div class="container mt-2">
    <div class="row">
      <div class="col">
        <the-header/>
      </div>
    </div>

    <div class="row mt-3">
      <div class="col-3">
        <the-sidebar/>
      </div>

      <div class="col-9">
        <account-index/>
      </div>

    </div>

    <div class="row mt-3">
      <div class="col">
        <the-footer/>
      </div>
    </div>
  </div>

</template>

<script>
import TheHeader from './TheHeader.vue';
import TheSidebar from './TheSidebar.vue';
import AccountIndex from './AccountIndex.vue';
import TheFooter from './TheFooter.vue';
export default {
  data() {
    return {}

  },
  components: {
    TheHeader,
    TheSidebar,
    AccountIndex,
    TheFooter,
  },
};
</script>


































