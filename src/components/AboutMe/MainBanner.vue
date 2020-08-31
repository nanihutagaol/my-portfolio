<template>
    <div class="x-banner">
        <div class="x-navbar">
            <ul>
                <li><a class="active" href="#home">Home</a></li>
                <!-- <li><a href="#news">News</a></li> -->
                <!-- <li><a href="#contact">Contact</a></li> -->
                <!-- <li><a href="#about">About</a></li> -->
            </ul>
        </div>

        <div class="x-banner-section">
            <div class="x-section-name">Hello! I'm {{name}}</div>
            <div class="x-section-tag">Fresh Graduate from Del Institute of Technology (IT Del)</div>
            <div class="x-section-suggest">This is my portfolio web.</div>
            <div class="x-section-button"><a href="#experience"><button class="btn">Let's Start</button></a></div>
        </div>        
    </div>
</template>

<script>

export default {
    name: 'MainBanner',
    props: {
        name: {
            type: String
        }
    }, 
    components: {
    } 
}
</script>

<style>
.x-banner {
    background-image: url("../../assets/work-desk.jpg");
    box-shadow: inset 0 0 0 1000px rgba(2, 57, 144, 0.5);
    padding: 0;
    margin-bottom: 1em;
    text-align: center;
}

.x-navbar {
    text-align: left;
    padding: 1.5em;
}

.x-navbar img {
    height: 48px;
}

.x-banner-section {
    color: #ffffff;
    padding: 5em 0 8.5em 0;
}

.x-section-name {
    font-size: 36px;
    font-weight: bold;
}

.x-section-tag {
    font-size: 26px;
}

.x-section-button button {
    border: 3px solid #ffffff;
    color: #ffffff;
    margin-top: 1.5em;
}
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
}

li {
  float: right;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover:not(.active) {
  text-decoration: none;
  color: #ddd;
}

li a.active, li a.onclick {
  font-weight: bold;
  text-decoration: none;
  color: white;
}
</style>