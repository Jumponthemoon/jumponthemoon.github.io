---
layout: about
title: About
permalink: /

show_posts: false
news: true
selected_papers: true
social: false

---

<style>
.post-header { display: none; }

.hero {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 4rem;
  align-items: stretch;
  margin: 1rem 0 1.5rem 0;
}
@media (max-width: 700px) {
  .hero { grid-template-columns: 1fr; }
}

/* Left column: profile card */
.hero .profile-card { display: flex; gap: 1.2rem; align-items: flex-start; }
.hero .profile-card .picture { flex: 0 0 160px; width: 160px; }
.hero .profile-card .info { min-width: 0; flex: 1 1 auto; }
.hero .profile-card .picture img {
  width: 160px; height: 160px;
  object-fit: cover; border-radius: 50%;
}
.hero .profile-card .info .name {
  font-size: 1.7rem; font-weight: 700; margin: 0 0 0.25rem 0; line-height: 1.1;
}
.hero .profile-card .info .role { color: #666; margin-bottom: 0.6rem; font-size: 0.9rem; }
.news table td, .news table th {
  padding-top: 1px !important;
  padding-bottom: 1px !important;
  line-height: 1.35;
}
.publications h2.bibliography { display: none; }
.research-callout {
  border-left: 3px solid #444;
  background: #f4f4f4;
  padding: 0.9rem 1.1rem;
  margin: 1.2rem 0;
  border-radius: 0 4px 4px 0;
  line-height: 1.55;
}
.publications { margin-top: 0.5rem !important; margin-bottom: 0.5rem !important; }
.services { margin-top: 1rem; }
article > h2 { margin-top: 0.5rem; margin-bottom: 0.6rem; }
.publications ol.bibliography li {
  margin-bottom: 0.4rem !important;
  line-height: 1.3;
}
.publications ol.bibliography li .abbr { margin-bottom: 0.15rem !important; }
.publications ol.bibliography li .title {
  font-family: "Inter", -apple-system, BlinkMacSystemFont, "Segoe UI", Arial, sans-serif !important;
  font-size: 0.95rem;
}
.publications ol.bibliography li .author {
  margin-bottom: 0.1rem;
  font-size: 0.85rem;
  font-weight: 300;
  color: #555;
}
.publications ol.bibliography li .author em {
  font-style: normal;
  font-weight: 700;
  text-decoration: underline;
  border-bottom: none !important;
  color: #1a1a1a;
}

.hero .role .caret {
  display: inline-block;
  animation: caretBlink 1s steps(1) infinite;
  margin-left: 1px;
}
@keyframes caretBlink { 50% { opacity: 0; } }
.hero .aff-label { font-weight: 600; margin-top: 0.15rem; font-size: 0.9rem; line-height: 1.2; }
.hero .aff {
  display: flex; align-items: center; gap: 0.4rem; margin: 0; font-size: 0.9rem; line-height: 1.2;
}
.hero .aff img { height: 18px; width: auto; }
.about-head {
  display: flex;
  align-items: center;
  gap: 0.8rem;
  margin-top: 0.5rem;
  margin-bottom: 0.6rem;
}
.about-head h2 { margin: 0 !important; }
.social-bar {
  display: flex;
  gap: 6px;
}
.social-bar a {
  display: inline-block; width: 30px; height: 30px; line-height: 30px;
  text-align: center;
  border: 2px solid var(--global-theme-color);
  border-radius: 4px;
  color: var(--global-theme-color);
  font-size: 13px;
  box-sizing: border-box;
}
.social-bar a:hover {
  background: var(--global-theme-color);
  color: #fff;
  text-decoration: none;
}
.hero .profile-card .info .social {
  margin-top: 0.7rem;
  margin-left: 0;
  padding-left: 0;
  display: flex;
  gap: 4px;
}
.hero .profile-card .info .social a {
  display: inline-block; width: 28px; height: 28px; line-height: 28px;
  text-align: center;
  border: 2px solid var(--global-theme-color);
  border-radius: 4px;
  margin-right: 3px;
  color: var(--global-theme-color);
  font-size: 12px;
  box-sizing: border-box;
}
.hero .profile-card .info .social a:hover {
  background: var(--global-theme-color);
  color: #fff;
}
.hero .profile-card .info .social a:hover { border-color: #bbb; text-decoration: none; }

.hero .right-col {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 1.2rem;
  align-items: stretch;
}
@media (max-width: 700px) {
  .hero .right-col { grid-template-columns: 1fr; }
}

/* Right column: research interests */
.hero .interests h3,
.hero .experience h3 {
  font-size: 0.78rem;
  font-weight: 600;
  letter-spacing: 0.18em;
  text-transform: uppercase;
  color: #888;
  border-bottom: none;
  padding-bottom: 0;
  margin-bottom: 0.6rem;
  font-family: "Inter", -apple-system, BlinkMacSystemFont, "Segoe UI", Arial, sans-serif !important;
}
.hero .interests ul { margin: 0; padding-left: 1.1rem; font-size: 0.9rem; }
.hero .interests li { margin-bottom: 0.2rem; }

/* Experience strip */
.experience {
  margin-bottom: 2rem;
}
.exp-list { list-style: none; padding: 0; margin: 0; }
.exp-list li {
  display: flex; justify-content: space-between;
  padding: 0.3rem 0;
  border-bottom: 1px dashed #eee;
}
.exp-list .role-org { font-weight: 600; }
.exp-list .time { color: #888; font-size: 0.9rem; }
</style>

<div class="hero">
  <div class="profile-card">
    <div class="picture">
      <img src="/assets/img/prof_pic.jpg" alt="profile photo">
    </div>
    <div class="info">
      <div class="name">Chenghao Qian</div>
      <div class="role">🌖 <a href="https://github.com/Jumponthemoon" style="color: inherit;"><span id="type-text"></span></a><span class="caret">|</span></div>

      <div class="aff-label">Ph.D. Student</div>
      <div class="aff">
        <img src="/assets/img/leeds_logo.png">
        <a href="https://uolds.leeds.ac.uk/">University of Leeds</a>
      </div>

      <div class="aff-label">Visiting Researcher</div>
      <div class="aff">
        <img src="/assets/img/cambridge_logo.png">
        <a href="https://www.cam.ac.uk/">University of Cambridge</a>
      </div>

    </div>
  </div>

  <div class="right-col">
    <div class="experience">
      <h3>Experience</h3>
      <div class="aff-label">Research Associate</div>
      <div class="aff">
        <img src="/assets/img/paralleldomain_logo.png">
        <a href="https://paralleldomain.com/">Parallel Domain</a>
      </div>
      <div class="aff-label">Sr. Algorithm Engineer</div>
      <div class="aff">
        <img src="/assets/img/xpeng_logo.png">
        <a href="https://www.xpeng.com/">XPENG Robotics</a>
      </div>
      <div class="aff-label">Algorithm Engineer</div>
      <div class="aff">
        <img src="/assets/img/ubtech_logo.png">
        <a href="https://www.ubtrobot.com/en/">UBTech Robotics</a>
      </div>
    </div>

    <div class="interests">
      <h3>Research Interests</h3>
      <ul>
        <li>Generative Simulation</li>
        <li>World Models</li>
        <li>Inverse Modelling</li>
        <li>Physics/Geometry-Guided Visual Generation</li>
      </ul>
    </div>
  </div>
</div>

<script>
(function() {
  const el = document.getElementById('type-text');
  if (!el) return;
  const text = 'jumponthemoon';
  let i = 0, deleting = false;
  function tick() {
    el.textContent = text.slice(0, i);
    if (!deleting) {
      if (i < text.length) { i++; setTimeout(tick, 80); }
      else { deleting = true; setTimeout(tick, 1800); }
    } else {
      if (i > 0) { i--; setTimeout(tick, 40); }
      else { deleting = false; setTimeout(tick, 500); }
    }
  }
  tick();
})();
</script>

<div class="about-head">
  <h2 id="about-me">About me</h2>
  <div class="social-bar">
    <a href="https://github.com/Jumponthemoon" title="GitHub"><i class="fab fa-github"></i></a>
    <a href="https://www.linkedin.com/in/chenghao-qian-021263240/" title="LinkedIn"><i class="fab fa-linkedin"></i></a>
    <a href="https://scholar.google.com/citations?user=EFV2q-4AAAAJ&hl=en" title="Google Scholar"><i class="ai ai-google-scholar"></i></a>
    <a href="https://www.photocrowd.com/photographer-community/293596/?page=images" title="Gallery"><i class="fas fa-camera"></i></a>
  </div>
</div>


I am currently pursuing a Ph.D. at <a href='https://uolds.leeds.ac.uk/'><u>Virtuocity</u></a>, and a visiting researcher at the <a href='https://www.cam.ac.uk/'><u>University of Cambridge</u></a>. Prior to this, I completed my master's degree at the <a href='https://www.sydney.edu.au/'><u>University of Sydney</u></a> and had industrial experience working in the fields of <strong style="color: #1772d0;">robotics</strong> and <strong style="color: #1772d0;">autonomous driving</strong> at <a href='https://paralleldomain.com/new-mcity-digital-twin-by-parallel-domain-brings-physical-ai-research-closer-to-reality'><u>Parallel Domain</u></a>, <a href='https://www.xpeng.com/'><u>XPENG</u></a> and <a href='https://www.ubtrobot.com/en/'><u>UBTech</u></a>.

<div class="research-callout">
My research bridges <strong style="color: #1772d0;">generative simulation</strong> and <strong style="color: #1772d0;">embodied agents</strong> to<br>build systems that <strong style="color: #1772d0;">👁️ perceive</strong>, <strong style="color: #1772d0;">🧠 reason</strong>, and <strong style="color: #1772d0;">🤖 act</strong> safely in the real world.
</div>

I am <strong style="color: #1772d0;">open to research collaborations</strong>. Please feel free to contact me at [tscq@leeds.ac.uk](mailto:tscq@leeds.ac.uk).

Beyond research, I’m into photography, basketball, and skateboarding.
