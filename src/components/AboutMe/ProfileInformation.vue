<template>
<div>
    <div class="x-profile">
        <img src="@/assets/foto-web.png">
        <h4 class="profile-name">Nani Renova Hutagaol</h4>
        <p class="profile-tag">Fresh Graduate<br> Del Institute of Technology (IT Del)</p>
        <p class="x-icon">
          <a href="https://www.linkedin.com/in/nani-renova-hutagaol-3ba350132/"><i class="fab fa-linkedin-in"></i></a>
          <a href="https://github.com/nanihutagaol"><i class="fab fa-github"></i></a>
        </p>
        <hr>
        <ul>
            <li><a class="active" href="#experience">Working Experiences</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#honors">Honors and Awards</a></li>
            <li><a href="#organizations">Organizations</a></li>
        </ul>
    </div>

    <div class="x-skill">
        <p class="x-card-title">Skills</p>
        <div class="x-card">
          <h4>Programming Language:</h4> 
          <p> C, C++, Java</p>
          
          <h4>Development:</h4> 
          <p>HTML, CSS, JavaScript, PHP, Yii2, VueJs, Docker </p>

          <h4>Database::</h4> 
          <p>MySQL, MongoDB</p>
        </div>
    </div>
</div>
</template>

<script>

export default {
    name: 'ProfileInformation',
    components: {

    }
}
</script>

<style>
.x-profile {
  line-height: 22px;
  text-align: center;
}

.x-profile img {
    height: 40%;
    border-radius: 50%;
    border: 3px solid #ddd;
    width: 75%;
}

.profile-name {
    margin-top: 1em;
    color: #3594dd;
    font-size: 28px;
}

.profile-tag {
    font-size: 14px;
    color: rgba(0,0,0,.6);
}

.x-profile ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  background-color: #f1f1f1;
}

.x-profile li {
    width: 100%;
}

.x-profile li a {
  display: block;
  color: #000;
  padding: 8px 16px;
  text-decoration: none;
  text-align: left;
  font-size: 16px;
}

.x-profile li a.active {
  background-color: #3594dd;
  color: white;
}

.x-profile li a:hover:not(.active) {
  background-color: #ddd;
  color: #000;
}

.x-skill {
  text-align: justify;
  margin-top: 1.5em;
  background-color: #f1f1f1;
  font-size: 16px;
}

.x-skill .x-card-title {
  background-color: #3594dd;
  padding: 0.5em 1em;
  color: white;
  font-weight: bold;
  font-size: 16px;
}

.x-skill .x-card {
  padding: 0 1em 1em 1em;
}

.x-skill .x-card h4 {
  font-size: 16px;
}
.x-icon a {
  padding: 0.5em;
}
.x-icon a i{
  font-size: 22px;
}
</style>