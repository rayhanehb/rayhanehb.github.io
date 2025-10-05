---
layout: default
title: About Me
permalink: /about.html
class: about-page
---

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

---

## 💼 Work & Research

<div class="experience">
  <img src="{{ site.baseurl }}/assets/img/sickkids_logo.png" alt="SickKids logo">
  <div>
    <h3>SickKids Hospital – Robotics Research Student</h3>
    <p>
      I was a research student at SickKids, where I worked on building a 
      simulation platform for robotic surgery. My focus was on connecting 
      the physical robot to its virtual model, troubleshooting issues like 
      synchronization delays and inverse kinematics mismatch, and testing 
      how virtual fixtures could guide more precise bone cutting.
    </p>
  </div>
</div>

<div class="experience">
  <img src="{{ site.baseurl }}/assets/img/geotab_logo.png" alt="Geotab logo">
  <div>
    <h3>Geotab – Embedded Systems Developer</h3>
    <p>
      I was an embedded systems developer at Geotab, working on the 
      firmware inside telematics devices used in fleet vehicles. I helped 
      design and implement new features, contributed to system-level 
      architecture, and built testing frameworks to make sure everything 
      held up at production scale.
    </p>
  </div>
</div>

<div class="experience">
  <img src="{{ site.baseurl }}/assets/img/pmcrt_logo.png" alt="UHN logo">
  <div>
    <h3>University Health Network – Computational Analyst</h3>
    <p>
      I was a computational analyst at UHN, where I worked with a 
      neuropathology lab to make large-scale data easier to use. I built 
      custom analysis tools so lab members without a programming 
      background could explore results independently, and I automated 
      workflows to support ongoing healthcare research.
    </p>
  </div>
</div>

---

## 🎨 Art, Engineering and Creativity

<p>
  Outside of engineering, I love exploring the ways art and technology overlap. In one of my favorite projects, I turned well-known ODE equations into an art piece by visualizing their solutions as particle motion in creative ways (you can read my full essay [here]({{site.baseurl}}/assets/docs/Exploring_Aesthetic_Theory_Through_the_Visual_Representation_of_ODEs.pdf)). I also loved my visit to teamLab Tokyo, where our hand-drawn sketches came to life on massive interactive screens. I would love to explore more projects that blend art and technology.
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

---

## 📫 Contact

<p>
📧 <a href="mailto:rayhaneh.behravesh@gmail.com">rayhaneh.behravesh@gmail.com</a><br>
💻 <a href="https://github.com/rayhanehb">GitHub</a><br>
💼 <a href="https://www.linkedin.com/in/r-behravesh">LinkedIn</a>
</p>

---

<style>
.about-page {
  max-width: 850px;
  margin: 40px auto;
  padding: 30px;
  background: #fff;
  border-radius: 12px;
  box-shadow: 0 2px 16px rgba(38,57,89,0.07);
  line-height: 1.6;
}

.about-header {
  margin-bottom: 40px;
}

.intro {
  display: flex;
  align-items: center;
  justify-content: center;
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
  box-shadow: 0 2px 8px rgba(38,57,89,0.12);
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
  width: 80px;           /* logo box size */
  height: 80px;
  object-fit: cover;      /* fill box, crop if needed */
  object-position: center; /* center cropped content */
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

<script>
  // Lightbox logic
  const galleryImages = document.querySelectorAll('.art-gallery img');
  const lightbox = document.getElementById('lightbox');
  const lightboxImg = document.getElementById('lightbox-img');
  const closeBtn = document.querySelector('.lightbox .close');

  galleryImages.forEach(img => {
    img.addEventListener('click', () => {
      lightbox.style.display = 'block';
      lightboxImg.src = img.src;
      lightboxImg.alt = img.alt;
    });
  });

  closeBtn.addEventListener('click', () => {
    lightbox.style.display = 'none';
  });

  lightbox.addEventListener('click', (e) => {
    if (e.target === lightbox) {
      lightbox.style.display = 'none';
    }
  });
</script>
