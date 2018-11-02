<template>
  <div class="update">
  <div style="height: 50px"></div>

  <form>
    <div class="form-group">
      <h3>Contact Info:</h3>
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
      <div style="height: 50px"></div>
      <h3>Short Bio:</h3>
      <textarea class="form-control" id="exampleFormControlTextarea1" rows="5"></textarea>
      <div style="height: 50px"></div>
      <h3>Experience:</h3>






      
      <h3>Education:</h3>
      Start Date: <br> 
      <input class="form-control form-control-sm" type="text" placeholder="Start Date">
      <div>
      End Date: <br>
      <input class="form-control form-control-sm" type="text" placeholder="End Date">
      </div>
      <div>
      Degree: <br>
      <input class="form-control form-control-sm" type="text" placeholder="Degree">
      </div>
      <div>
      University Name: <br>
      <input class="form-control form-control-sm" type="text" placeholder="University Name">
      </div>
      Details: <br>
      <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
      <br><br>





      <h3>Skills:</h3>






      <h3>Capstone:</h3>




      


      





              <input type="submit" class="btn btn-primary" value="Submit">

           

 
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
      newExperience: [ 
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
      newEducation: [
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
  created: function() {},
  methods: {
    addExperience: function() {
      var params = {
                    startDate: this.newExperience
      }
    }
  },
  computed: {}
};
</script>