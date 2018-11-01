<template>
  <div class="update">
    <h1>this is the update page</h1>

  <form>

    <div class="form-group">
      <h3>Student Attributes</h3>
      First Name: <br>
      <input class="form-control" type="text" placeholder="First Name">
      Last Name:  <br>
      <input class="form-control" type="text" placeholder="Last Name">
      Email: <br>
      <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Enter Email">
      Phone Number: <br>
      <input class="form-control" type="tel" placeholder="555-555-5555">
      Short Bio: <br>
      <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
      LinkedIn URL <br>
      <input class="form-control" type="url" placeholder="https://www.linkedin.com/in/hommer-zollenger/">
      Twitter Handle:  <br>
      <input class="form-control" type="text" placeholder="@homerZZZZ">
      Personal Blog/Website URL <br>
      <input class="form-control" type="url" placeholder="https://www.homeskoolkids.com/">
      






      
    
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
      student: [ 
      {
        studentName: "",
        email: "",
        phoneNumber: "",
        shortBio: "",
        linkinUrl: "",
        twitter: "",
        personalWebsite: "",
        onlineResume: "",
        github: "",
        photoImg: "",
      }],
      experience: [ 
      {
        startDate: "",
        endDate: "",
        jobTitle: "",
        companyName: "",
        details: "",
      }],
      education: [
      {
      startDate: "",
      endDate: "",
      degree: "",
      universityName: "",
      }],
      skillName: "",
      capstone: [
      {
      name: "",
      description: "",
      url: "",
      
      }]
     
    };

  },
  created: function() {

  },
  methods: {},
  computed: {}
};
</script>