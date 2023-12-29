<template>

  <section class="head row justify-content-between align-items-center">
    <div class="col-auto"><a href="#">Logo</a></div>
    <div class="col-auto d-flex align-items-center">
      <div class="d-inline-block avatar"></div>
      <div class="d-inline-block nickname"><a href="#">{{ account.nickname }}</a></div>
    </div>
  </section>

</template>

<script>
import {mapState} from "pinia";
import {useAccountStore} from './stores/account.js';

export default {
  name: 'TheHeader',
  data() {
    return {}
  },
  computed: {
    ...mapState(useAccountStore, ['account']),

  }
};
</script>

<style>
.head {
  padding: 10px;
  border: 1px solid blue;

}

.avatar {
  margin-right: 10px;
  padding: 10px;
  border: 1px solid cadetblue;
  border-radius: 50px;
  background: cadetblue;
}
</style>