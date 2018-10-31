<template>
  <div class="update">
    <h1>this is the update page</h1>

  <form>
 
 <h1>Login</h1>
        <ul>
          <li class="text-danger" v-for="error in errors">{{ error }}</li>
        </ul>

<div>  
<input class="form-control form-control-sm" type="text" placeholder="Start Date">
</div>


        <input type="submit" class="btn btn-primary" value="Submit">

    <div class="form-group">
      <label for="exampleFormControlTextarea1">Example textarea</label>
      <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
    </div>
  </form>
  </div>

</template>

<style>
</style>

<script>
import axios from "axios";

export default {
  template: "#login-page",
  data: function() {
    return {
      email: "",
      password: "",
      errors: []
    };
  },
  methods: {

  },
  computed: {}
};
</script>