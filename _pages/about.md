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
.hero .profile-card .info .role {
  color: var(--global-text-color);
  margin-bottom: 0.6rem;
  font-size: 0.85rem;
  font-family: "JetBrains Mono", "Fira Code", "Menlo", "Consolas", monospace;
  font-weight: 500;
  letter-spacing: 0.02em;
}
.hero .profile-card .info .role .prompt { color: #17a05f; font-weight: 700; }
.news table td, .news table th {
  padding-top: 1px !important;
  padding-bottom: 1px !important;
  line-height: 1.6;
  font-family: "Inter", -apple-system, BlinkMacSystemFont, "Segoe UI", Arial, sans-serif !important;
  font-size: 1rem;
  font-weight: 400;
  letter-spacing: 0.005em;
  word-spacing: normal;
}
.news table td a {
  font-family: inherit !important;
  font-weight: inherit;
}
.publications h2.bibliography { display: none; }
.publications ol.bibliography li .abbr abbr {
  background-color: #0e2540 !important;
}
.research-callout {
  border-top: 1px solid #d8d8d8;
  border-bottom: 1px solid #d8d8d8;
  background: rgba(0, 0, 0, 0.02);
  padding: 1.2rem 1.4rem;
  margin: 1.6rem 0;
  line-height: 1.6;
  text-align: center;
  font-size: 1.02rem;
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
  color: #888;
}
html[data-theme="dark"] .publications ol.bibliography li .author {
  color: #bbb;
}
.publications ol.bibliography li .author em {
  font-style: normal;
  font-weight: 700;
  text-decoration: underline;
  border-bottom: none !important;
  color: #888;
}
html[data-theme="dark"] .publications ol.bibliography li .author em {
  color: #bbb;
}

.hero .role .caret {
  display: inline-block;
  animation: caretBlink 1.1s cubic-bezier(0.4, 0, 0.2, 1) infinite;
  margin-left: 1px;
}
@keyframes caretBlink {
  0%, 45% { opacity: 1; }
  50%, 95% { opacity: 0; }
  100% { opacity: 1; }
}
.aff-label { font-weight: 600; margin-top: 0.5rem; font-size: 0.9rem; line-height: 1.4; color: #888; }
html[data-theme="dark"] .aff-label { color: #bbb; }
.aff {
  display: flex; align-items: center; gap: 0.4rem; margin: 0.1rem 0; font-size: 0.9rem; line-height: 1.4;
}
.aff img { height: 18px; width: auto; }
.experience .aff { margin: 0.3rem 0; }
/* One shared grid for all Experience rows, so the separator and the role line
   up in columns instead of trailing company names of different lengths. */
.experience .aff-list {
  display: grid;
  grid-template-columns: max-content max-content max-content max-content;
  align-items: center;
  column-gap: 0.4rem;
  row-gap: 0.3rem;
}
.experience .aff-list .aff { display: contents; }
.experience .aff-list .role-sep { margin: 0; }
.aff-role { color: #888; font-weight: 400; }
html[data-theme="dark"] .aff-role { color: #bbb; }
.role-sep { color: #aaa; margin: 0 0.3rem; }
.about-head {
  display: flex;
  align-items: center;
  gap: 0.8rem;
  margin: 0 0 0.5rem 0;
  min-height: 1.7rem;
}
.hero .right-col .about-head h2 {
  margin: 0 !important;
  padding: 0 !important;
  line-height: 1.1;
  font-size: 1.7rem;
}
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
  display: flex;
  flex-direction: column;
  padding: 0;
  margin: 0;
  align-self: stretch;
}
.hero .right-col > *:first-child { margin-top: 0 !important; padding-top: 0 !important; }
.hero .right-col p {
  margin: 0;
  line-height: 1.6;
  margin-top: auto;
}

/* Right column: research interests */
.interests h3,
.experience h3 {
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
.interests ul {
  margin: 0;
  padding-left: 1.1rem;
  font-size: 0.9rem;
  list-style: disc;
  line-height: 1.2;
}
.interests li { margin: 0; padding: 0; }

/* Below-hero two-column block */
.below-hero {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 2.5rem;
  margin: 2rem 0;
}
@media (max-width: 700px) {
  .below-hero { grid-template-columns: 1fr; }
}

/* Experience strip */
.experience {
  margin-bottom: 0;
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
      <div class="role"><i class="fab fa-github" style="color: var(--global-text-color); font-size: 1.05em;"></i> <a href="https://github.com/Jumponthemoon" style="color: inherit;"><span id="type-text"></span></a><span class="caret">_</span></div>

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
    <div class="about-head">
      <h2 id="about-me">About me</h2>
      <div class="social-bar">
        <a href="https://github.com/Jumponthemoon" title="GitHub"><i class="fab fa-github"></i></a>
        <a href="https://www.linkedin.com/in/chenghao-qian-021263240/" title="LinkedIn"><i class="fab fa-linkedin"></i></a>
        <a href="https://scholar.google.com/citations?user=EFV2q-4AAAAJ&hl=en" title="Google Scholar"><i class="ai ai-google-scholar"></i></a>
        <a href="https://www.photocrowd.com/photographer-community/293596/?page=images" title="Gallery"><i class="fas fa-camera"></i></a>
      </div>
    </div>
    <p>I am currently pursuing a Ph.D. at <a href='https://uolds.leeds.ac.uk/'><u>Virtuocity</u></a>, and a visiting researcher at the <a href='https://www.cam.ac.uk/'><u>University of Cambridge</u></a>. I completed my master's degree at the <a href='https://www.sydney.edu.au/'><u>University of Sydney</u></a> and had industrial experience working in the fields of <strong style="color: #1772d0;">robotics</strong> and <strong style="color: #1772d0;">autonomous driving</strong>.</p>
  </div>
</div>

{% comment %}
  Research callout temporarily hidden -- delete this comment wrapper to bring it back.
{% endcomment %}
{% comment %}
<div class="research-callout">
My works aim to bridge <strong style="color: #1772d0;">generative models</strong> and <strong style="color: #1772d0;">embodied agents</strong> to<br>build systems that <strong style="color: #1772d0;">👁️ perceive</strong>, <strong style="color: #1772d0;">🧠 reason</strong>, and <strong style="color: #1772d0;">🤖 act</strong> safely in the real world.
</div>
{% endcomment %}

<div class="below-hero">
  <div class="experience">
    <h3>Experience</h3>
    <div class="aff-list">
      <div class="aff">
        <img src="/assets/img/paralleldomain_logo.png">
        <a href="https://paralleldomain.com/">Parallel Domain</a>
        <span class="role-sep">·</span>
        <span class="aff-role">Research Intern</span>
      </div>
      <div class="aff">
        <img src="/assets/img/xpeng_logo.png">
        <a href="https://www.xpeng.com/">XPENG Robotics</a>
        <span class="role-sep">·</span>
        <span class="aff-role">Sr. Algorithm Engineer</span>
      </div>
      <div class="aff">
        <img src="/assets/img/ubtech_logo.png">
        <a href="https://www.ubtrobot.com/en/">UBTech Robotics</a>
        <span class="role-sep">·</span>
        <span class="aff-role">Algorithm Engineer</span>
      </div>
    </div>
  </div>

  <div class="interests">
    <h3>Research Interests</h3>
    <ul>
      <li>3D & Video World Models</li>
      <li>Physics-guided Generation</li>
      <li>Inverse Modelling</li>
      <li>Robust Perception</li>
    </ul>
  </div>
</div>


<script>
(function() {
  const el = document.getElementById('type-text');
  if (!el) return;
  const text = 'jumponthemoon';
  let i = 0, deleting = false;
  const rand = (a, b) => a + Math.random() * (b - a);
  function tick() {
    el.textContent = text.slice(0, i);
    let delay;
    if (!deleting) {
      if (i < text.length) { i++; delay = rand(60, 130); }
      else { deleting = true; delay = 2200; }
    } else {
      if (i > 0) { i--; delay = rand(25, 55); }
      else { deleting = false; delay = 600; }
    }
    setTimeout(tick, delay);
  }
  tick();
})();
</script>

I am <strong style="color: #1772d0;">open to research collaborations</strong>. Please feel free to contact me at <a href="mailto:tscq@leeds.ac.uk" style="color: #1772d0;">tscq@leeds.ac.uk</a>.
