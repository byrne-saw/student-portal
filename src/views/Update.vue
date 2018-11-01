<template>
  <div class="update">
  <div style="height: 50px"></div> 

  <form>
    <div class="form-group">
      <h3>Student Attributes</h3>
      <div class="row">
        <div class="col">
          First Name: <br> <input class="form-control" type="text" placeholder="First Name">
        </div>
        <div class="col">
          Last Name: <br> <input class="form-control" type="text" placeholder="Last Name">
        </div>
      </div>
      <div class="row">
        <div class="col">
          Email: <br> <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Enter Email">
        </div>
        <div class="col">
          Phone Number: <br> <input class="form-control" type="tel" placeholder="555-555-5555">
        </div>
      </div>
      <div class="row">
        <div class="col">
          LinkedIn URL <br> <input class="form-control" type="url" placeholder="https://www.linkedin.com/in/hommer-zollenger/">
        </div>
        <div class="col">
          Twitter Handle: <br> <input class="form-control" type="text" placeholder="@homerZZZZ">
        </div>        
      </div>
      <div class="row">
        <div class="col">
          Personal Blog/Website URL <br> <input class="form-control" type="url" placeholder="https://www.homeskoolkids.com/">
        </div>
        <div class="col">
          Online Resume URL <br> <input class="form-control" type="url" placeholder="https://www.dope_resumes.com/">
        </div>
      </div>
      <div class="row">
        <div class="col">
          Github URL <br> <input class="form-control" type="url" placeholder="https://github.com/you">
        </div>
        <div class="col">
          Photo URL <br> <input class="form-control" type="url" placeholder="https://www.imgur.com/your_photo">
        </div>
      </div>
      Short Bio: <br> <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>

      






      
    
    </div>
    
  </form>
  </div>

</template>

<style>
</style>

<script>
export default {
  data: function() {
    return {
    };
  },
  created: function() {},
  methods: {},
  computed: {}
};
</script>