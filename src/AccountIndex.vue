<template>

  <div class="index row ps-3 align-content-start">
    <div class="col-8">
      <h2>My account</h2>
    </div>

    <div class="col-4 text-end">
      <button class="btn btn-warning btn-sm" @click="showForm = true">Edit</button>
    </div>

    <div class="col-12">
      FullName: [full-name]
    </div>

    <div class="col-12">
      Nickname: {{ account.nickname }}
    </div>

    <div class="col-12">
      About: [about]
    </div>

  </div>

  <account-form v-model="showForm"/>

</template>

<script>
import {mapState} from "pinia";
import {useAccountStore} from './stores/account.js';
import AccountForm from "./AccountForm.vue";

export default {
  name: 'AccountIndex',
  components: {AccountForm},
  data() {
    return {
      showForm: false,
    };
  },
  computed: {
    ...mapState(useAccountStore, ['account']),
  },
}
</script>

<style>
.index {
  color: black;
}
</style>