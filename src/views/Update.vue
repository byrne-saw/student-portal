<template>
  <div class="update">
  <div style="height: 50px"></div>

  <form>
    <div class="form-group">
      <h3>Contact Info:</h3>
      <div class="row">
        <div class="col">
          First Name: <br> <input class="form-control" type="text" v-bind:placeholder="student.studentName">
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
      <div style="height: 50px"></div>
      <h3>Short Bio:</h3>
      <textarea class="form-control" id="exampleFormControlTextarea1" rows="5"></textarea>
      <div style="height: 50px"></div>

      <h3>Experience:</h3>
      <div class="row">
        <div class="col">
          Company Name: <br><input class="form-control form-control-sm" type="text" placeholder="University Name">
        </div>
        <div class="col">
          Job Title: <br><input class="form-control form-control-sm" type="text" placeholder="University Name">
        </div>
      </div>
      <div class="row">
        <div class="col">
          Start Date:<br> <input class="form-control form-control-sm" type="text" placeholder="Start Date">
        </div>
        <div class="col">
          End Date: <br> <input class="form-control form-control-sm" type="text" placeholder="End Date">
        </div>
      </div>
      Details: <br><textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>

      <div style="height: 50px"></div>
      
      <h3>Education:</h3>
      University Name: <br><input class="form-control form-control-sm" type="text" placeholder="University Name">
      <div class="row">
        <div class="col">
          Start Date:<br> <input class="form-control form-control-sm" type="text" placeholder="Start Date">
        </div>
        <div class="col">
          End Date: <br> <input class="form-control form-control-sm" type="text" placeholder="End Date">
        </div>
      </div>
      Degree: <br>
      <input class="form-control form-control-sm" type="text" placeholder="Degree">
      Details: <br><textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
      <div style="height: 50px"></div>

      

      <h3>Skills:</h3>
      Skills: <br><input class="form-control form-control-sm" type="text" placeholder="Skill">
      <div style="height: 50px"></div>
      
      <h3>Capstone:</h3>
      <div class="row">
        <div class="col">
          Name: <br> <input class="form-control" type="text" placeholder="student.studentName">
        </div>
        <div class="col">
          URL: <br> <input class="form-control" type="text" placeholder="url">
        </div>
      </div>
      Description: <br><textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
      Screenshot URL: <br> <input class="form-control" type="url" placeholder="https://www.imgur.com/your_photo">
      <div style="height: 50px"></div>
      <input type="submit" class="btn btn-primary" value="Submit">

    </div>
  </form>
  </div>

</template>

<style>
</style>

<script>
var axios = require('axios');

export default {
  data: function() {
    return {

      students: {},
          
    };
  },
  created: function() {
    axios
      .get("https://blooming-caverns-85738.herokuapp.com/api/students/2")
      .then(response => {
        this.students = response.data;
      });
    console.log(this.students);
  },
  methods: {
    // submitData: function() {
    //   this.errors = [];
    //   var params = {
    //                 name: this.newPerson.name,
    //                 bio: this.newPerson.bio
    //                 };
    //   axios
    //     .post("http://localhost:3000/api/people", params)
    //     .then(response => {
    //       this.people.push(response.data);
    //       this.newPerson = {name: "", bio: "", bioVisible: false};
    //     })
    //     .catch(error => {
    //       this.errors = error.response.data.errors;
    //     });
    // },
  },

  computed: {}
};
</script>