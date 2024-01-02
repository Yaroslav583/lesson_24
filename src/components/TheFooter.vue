<template>

  <section class="footer row">
    <div class="col">
      <ul class="list-group list-group-horizontal nav text-center w-100 justify-content-center ">
        <li class="list-group-item"><a href="#">Home</a></li>
        <li class="list-group-item"><a href="#">News</a></li>
        <li class="list-group-item"><a href="#">Feed</a></li>
        <li class="list-group-item"><a href="#">My account</a></li>
        <li class="list-group-item"><a href="#">Settings</a></li>
      </ul>
    </div>
  </section>

</template>

<script>
export default {
  name: 'TheFooter',
  data() {
    return {}

  },
};
</script>


<style>
.footer {
  margin-top: 450px;
  padding: 10px;
  border: 1px solid blue;
}
</style>