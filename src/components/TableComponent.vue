<template>
  <div>
    <table class="table table-striped">
      <thead>
        <tr>
          <th>#</th>
          <th>Name</th>
          <th>City</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="user in Data">
          <td>{{ user.id }}</td>
          <td>{{ user.name }}</td>
          <td>{{ user.city }}</td>
        </tr>
        <tr>
          <td class="total" colspan="3">
            total number of students is : {{ Data.length }}
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
import Data from "@/Data";
export default {
  data() {
    return {
      Data: Data,
    };
  },
};
</script>

<style scoped>
.total {
  text-transform: capitalize;
  text-align: center;
  background-color: #3cb371;
  color: #fff !important;
  font-weight: bold;
}
</style>
