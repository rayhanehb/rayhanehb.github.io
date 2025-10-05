---
layout: default
title: About Me
permalink: /about.html
class: about-page
---

<!-- Sidebar -->
<aside class="sidebar">
  <header>
    <div class="about">
      <div class="cover-author-image">
        <a href="{{site.baseurl}}/">
          <img src="{{site.baseurl}}/assets/img/{% if site.author-img %}{{site.author-img}}{% endif %}" alt="{{site.author}}">
        </a>
      </div>
      <div class="author-name">{{site.author}}</div>
      <p>{{site.about-author}}</p>
    </div>
  </header>
  <footer>
    <section class="contact">
      <h3 class="contact-title">Contact me</h3>
      <ul>
        <li><a href="http://github.com/{{site.social-github | default: ''}}" target="_blank"><i class="fa fa-github"></i></a></li>
        <li><a href="http://www.linkedin.com/in/r-behravesh" target="_blank"><i class="fa fa-linkedin"></i></a></li>
        <li><a href="mailto:rayhaneh.behravesh@gmail.com"><i class="fa fa-envelope-o"></i></a></li>
      </ul>
    </section>
    <div class="copyright">
      <p>{{site.time | date: '%Y'}} &copy; {{site.author}}</p>
    </div>
  </footer>
</aside>

<!-- Navigation -->
<nav class="main-nav">
  <ul>
    <li><a href="{{ site.baseurl }}/">Home</a></li>
    <li><a href="{{ site.baseurl }}/about.html">About Me</a></li>
  </ul>
</nav>

<!-- Main content -->
<div class="content-box clearfix">

  <div class="about-header">
    <div class="intro">
      <img src="{{ site.baseurl }}/assets/img/rayhaneh_about.png" alt="Rayhaneh Behravesh" class="profile-pic">
      <div class="intro-text">
        <h1>Hi, I’m Rayhaneh 👋</h1>
        <p>
          I’m currently a graduate student in <strong>Robotics at Johns Hopkins University</strong>, 
          and I completed my <strong>Engineering Science degree at the University of Toronto</strong>. 
        </p>
        <p>
          I enjoy meeting people who share interests in robotics, art, or just fun ideas in general. 
          Feel free to reach out! You can email me at 
          <a href="mailto:rayhaneh.behravesh@gmail.com">rayhaneh.behravesh@gmail.com</a> or connect with me on 
          <a href="https://www.linkedin.com/in/r-behravesh">LinkedIn</a>.
        </p>
      </div>
    </div>
  </div>

  <!-- Work & Research -->
  <h2>💼 Work & Research</h2>

  <div class="experience">
    <img src="{{ site.baseurl }}/assets/img/sickkids_logo.png" alt="SickKids logo">
    <div>
      <h3>SickKids Hospital – Robotics Research Student</h3>
      <p>
        I was a research student at SickKids, building a simulation platform for robotic surgery. 
        I connected the physical robot to its virtual model, addressed synchronization delays 
        and inverse kinematics mismatches, and tested virtual fixtures to guide precise bone cutting.
      </p>
    </div>
  </div>

  <div class="experience">
    <img src="{{ site.baseurl }}/assets/img/geotab_logo.png" alt="Geotab logo">
    <div>
      <h3>Geotab – Embedded Systems Developer</h3>
      <p>
        I worked on the firmware inside telematics devices for fleet vehicles, 
        contributing to system-level architecture, implementing new features, 
        and building testing frameworks to ensure production reliability.
      </p>
    </div>
  </div>

  <div class="experience">
    <img src="{{ site.baseurl }}/assets/img/pmcrt_logo.png" alt="UHN logo">
    <div>
      <h3>University Health Network – Computational Analyst</h3>
      <p>
        I helped a neuropathology lab make large-scale data more accessible. 
        I built analysis tools for non-programmers and automated workflows to support ongoing healthcare research.
      </p>
    </div>
  </div>

  <!-- Art Section -->
  <h2>🎨 Art, Engineering and Creativity</h2>
  <p>
    I love exploring how <em>art and technology</em> intersect.  
    One of my favorite projects was turning an <strong>ODE assignment</strong> into an art piece by visualizing particle motion
    (you can read the full essay <a href="{{site.baseurl}}/assets/docs/Exploring_Aesthetic_Theory_Through_the_Visual_Representation_of_Ordinary_Differential_Equations.pdf">here</a>).  
    I also visited <strong>teamLab Tokyo</strong>, where our hand-drawn sketches came to life on interactive screens.
  </p>

  <div class="art-gallery">
    <img src="{{ site.baseurl }}/assets/img/ODE_annotated.png" alt="ODE Project">
    <img src="{{ site.baseurl }}/assets/img/teamlab_drawing.png" alt="TeamLab Drawing">
    <img src="{{ site.baseurl }}/assets/img/drawing_tazhib.png" alt="Tazhib Drawing">
    <img src="{{ site.baseurl }}/assets/img/drawing_bird.png" alt="Bird Drawing">
  </div>

  <!-- Lightbox overlay -->
  <div id="lightbox" class="lightbox">
    <span class="close">&times;</span>
    <img class="lightbox-content" id="lightbox-img">
  </div>


</div>

<!-- Styles -->
<style>
.about-page {
  max-width: 850px;
  margin: 40px auto;
  padding: 30px;
  background: #fff;
  border-radius: 12px;
  box-shadow: 0 2px 6px rgba(38,57,89,0.05);
  line-height: 1.6;
}

.about-header {
  margin-bottom: 40px;
}

.intro {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  gap: 25px;
  max-width: 750px;
  margin: 0 auto;
  text-align: left;
  flex-wrap: wrap;
}

.profile-pic {
  width: 140px;
  height: 140px;
  border-radius: 50%;
  object-fit: cover;
  box-shadow: 0 2px 6px rgba(38,57,89,0.08);
  flex-shrink: 0;
}

.intro-text {
  flex: 1;
  min-width: 250px;
}

.intro-text h1 {
  margin-top: 0;
  margin-bottom: 0.4em;
  font-size: 2em;
  color: #263959;
}
.intro-text p {
  margin: 0.5em 0;
  font-size: 1.05em;
  line-height: 1.6;
}

.experience {
  display: flex;
  align-items: flex-start;
  margin-bottom: 30px;
  flex-wrap: nowrap;
}

.experience img {
  width: 80px;
  height: 80px;
  object-fit: cover;
  object-position: center;
  margin-right: 16px;
  border-radius: 6px;
  box-shadow: 0 1px 3px rgba(38,57,89,0.1);
}

.art-gallery {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
  gap: 16px;
  justify-items: center;
  margin: 24px 0;
}

.art-gallery img {
  width: 100%;
  max-width: 180px;
  aspect-ratio: 1 / 1;
  object-fit: cover;
  border-radius: 10px;
  box-shadow: 0 1px 6px rgba(38,57,89,0.1);
  background: #fafbfc;
  cursor: pointer;
  transition: transform 0.2s;
}
.art-gallery img:hover {
  transform: scale(1.05);
}

/* Lightbox styles */
.lightbox {
  display: none;
  position: fixed;
  z-index: 999;
  padding-top: 60px;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  overflow: auto;
  background-color: rgba(0,0,0,0.85);
}

.lightbox-content {
  display: block;
  margin: auto;
  max-width: 80%;
  max-height: 80%;
  border-radius: 10px;
  box-shadow: 0 2px 12px rgba(0,0,0,0.4);
}

.lightbox .close {
  position: absolute;
  top: 20px;
  right: 35px;
  color: #fff;
  font-size: 36px;
  font-weight: bold;
  cursor: pointer;
}
</style>

<!-- Lightbox script -->
<script>
const galleryImages = document.querySelectorAll('.art-gallery img');
const lightbox = document.getElementById('lightbox');
const lightboxImg = document.get
