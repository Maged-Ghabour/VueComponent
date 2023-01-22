<template>
  <div class="header text-center">
    <div class="container">
      <HeaderComponent />
    </div>
  </div>
  <div class="container">
    <div class="row mt-2">
      <div class="col-4"><NavComponent /></div>
      <div class="col-8"><TableComponent /></div>
    </div>
  </div>
  <div class="footer">
    <div class="container">
      <FooterComponent />
    </div>
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import NavComponent from "./components/NavComponent.vue";
import TableComponent from "./components/TableComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";
export default {
  data() {
    return {};
  },
  components: {
    HeaderComponent,
    NavComponent,
    TableComponent,
    FooterComponent,
  },
};
</script>

<style>
.header,
.footer {
  background-color: mediumseagreen;
}
</style>
