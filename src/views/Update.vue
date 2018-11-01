<template>
  <div class="update">
    <h1>this is the update page</h1>

  <form>
    <div class="form-group">
      <label for="exampleFormControlInput1">Email address</label>
      <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="name@example.com">
    </div>
    <div class="form-group">
      <label for="exampleFormControlSelect1">Example select</label>
      <select class="form-control" id="exampleFormControlSelect1">
        <option>1</option>
        <option>2</option>
        <option>3</option>
        <option>4</option>
        <option>5</option>
      </select>
    </div>
    <div class="form-group">
      <label for="exampleFormControlSelect2">Example multiple select</label>
      <select multiple class="form-control" id="exampleFormControlSelect2">
        <option>1</option>
        <option>2</option>
        <option>3</option>
        <option>4</option>
        <option>5</option>
      </select>
    </div>
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
export default {
  data: function() {
    return {
      student: [
        first_name:
        email: "",
        phone_number: "",
        short_bio: "",
        linkin_url: "",
        twitter: "",
        personal_website: "",
        online_resume: ""
        github: ""
        photo_img: 
      ],
      experience: [
        start_date: "",
        end_date: "",
        job_title: "",
        company_name: ""
        details: ""
      ],
      education: [
      start_date: "",
      end_date: "",
      degree: "",
      university_name: "",
      ],
      skill_name: "",
      capstone: [
      name: "",
      description: "",
      url: "",
      
      ]
     
    };

  },
  created: function() {},
  methods: {},
  computed: {}
};
</script>