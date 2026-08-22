---
layout: page
title: ViBe
page_title: ViBe - The Future of Learning
parent: Products
order: 1
---


*Like Vikram with Betaal at every stride,*
*ViBe questions you–till trust and confidence walk by your side.*


ViBe launched on 29th July 2025, when Education Minister Shri Dharmendra Pradhan unveiled it at the Akhil Bharatiya Shiksha Samagam. It's open-source and free to use, built and kept running by a community of developers and educators. You can look at the code or help build it on our [GitHub Repository](https://github.com/vicharanashala/vibe).

---

## **About**

<div class="split-media">
<p>ViBe turns passive video-watching into active learning. It gives students a clear, step-by-step way to learn, gives teachers useful insights without extra work, and is built so students trust the process and feel sure about what they know.</p>

{% include video-thumb.html id="6AYCVKDIeTs" title="ViBe – Concept Video" %}
</div>

---

## **Who It's For**

<div class="audience-grid">
  <div class="audience-card">
    <i class="ph ph-graduation-cap audience-card-icon"></i>
    <div class="audience-card-title">Students</div>
    <p class="audience-card-desc">Learn in short video segments with quizzes built in. Earn points, track your own progress, ask questions right on the video, and get instant help from an AI assistant.</p>
  </div>
  <div class="audience-card">
    <i class="ph ph-chalkboard-teacher audience-card-icon"></i>
    <div class="audience-card-title">Teachers</div>
    <p class="audience-card-desc">Turn any video or playlist into a full course. ViBe splits it into parts, writes a transcript, and drafts quiz questions for you to check. Manage your students, invites, and announcements from one place.</p>
  </div>
</div>

---

## **The Challenge**

Online courses are easy to access but hard to finish. Most self-paced video courses see only 10 to 15 percent of learners complete them. Most platforms just show the video and hope learning happens. Without a teacher watching, students often let the video play without really following it. The challenge is building a system that keeps learners accountable without making them feel watched or anxious.

---

## **The Platform**

ViBe takes its name from the old tale of Vikram and Betaal, where a wrong answer means going back and trying again. ViBe works the same way: it checks how well you understand something as you go, and asks you to revisit anything you missed.

{% include video-thumb.html id="8ytNdYlK-BU" title="ViBe – Interactive Demo" %}

<div class="audience-grid">
  <div class="audience-card">
    <i class="ph ph-scissors audience-card-icon"></i>
    <div class="audience-card-title">Micro-Learning</div>
    <p class="audience-card-desc">Long lectures are automatically split into short parts, one idea at a time, so you're never overwhelmed.</p>
  </div>
  <div class="audience-card">
    <i class="ph ph-target audience-card-icon"></i>
    <div class="audience-card-title">Smart Assessments</div>
    <p class="audience-card-desc">Quizzes pop up during the video, not after it, so you're tested while it's still fresh, not days later.</p>
  </div>
  <div class="audience-card">
    <i class="ph ph-shield-check audience-card-icon"></i>
    <div class="audience-card-title">Active Verification</div>
    <p class="audience-card-desc">AI watches for signs you've lost focus, like switching tabs or looking away, without making it feel like it's spying on you.</p>
  </div>
  <div class="audience-card">
    <i class="ph ph-users-three audience-card-icon"></i>
    <div class="audience-card-title">ViBeCrowd</div>
    <p class="audience-card-desc">Learners help write and check quiz questions together, so the question bank keeps getting better.</p>
  </div>
  <div class="audience-card">
    <i class="ph ph-magic-wand audience-card-icon"></i>
    <div class="audience-card-title">AI Course Generation</div>
    <p class="audience-card-desc">Give ViBe a video or playlist and it builds a course from it: splitting it into parts, writing a transcript, and drafting quiz questions. The teacher checks and approves each step. Or just share one video and see who watched it.</p>
  </div>
  <div class="audience-card">
    <i class="ph ph-trophy audience-card-icon"></i>
    <div class="audience-card-title">Community & Recognition</div>
    <p class="audience-card-desc">Earn points, see how you rank against classmates, ask questions right on the video, and share how you're feeling about each lesson.</p>
  </div>
</div>

---

## **See It In Action**

A look at the real product – swipe through the screens students and teachers actually use.

<div class="shot-carousel" id="vibe-shot-carousel">
  <div class="shot-slide active">
    <img src="{{ site.baseurl }}/assets/images/vibe/student-dashboard.jpg" alt="ViBe student dashboard showing enrolled and completed courses">
    <figcaption>Student dashboard – courses, progress, and what to pick up next.</figcaption>
  </div>
  <div class="shot-slide">
    <img src="{{ site.baseurl }}/assets/images/vibe/student-analytics.jpg" alt="ViBe learning analytics dashboard showing progress, quiz performance, and content completion">
    <figcaption>Learning Analytics – every learner sees their own progress, pace, and quiz performance.</figcaption>
  </div>
  <div class="shot-slide">
    <img src="{{ site.baseurl }}/assets/images/vibe/student-leaderboard.jpg" alt="ViBe cohort leaderboard ranking learners by completion speed and weekly effort">
    <figcaption>Cohort leaderboard – ranked by completion speed and this week's effort.</figcaption>
  </div>
  <div class="shot-slide">
    <img src="{{ site.baseurl }}/assets/images/vibe/teacher-share-video.jpg" alt="ViBe Share a Video screen for sending a watch-tracked video link">
    <figcaption>Share a video – a watch-tracked link, no full course required.</figcaption>
  </div>
  <div class="shot-slide">
    <img src="{{ site.baseurl }}/assets/images/vibe/teacher-course-management.jpg" alt="ViBe course version management panel with flags, enrollments, registrations, and ejection policy controls">
    <figcaption>Per-course controls – flags, enrollments, registrations, and ejection policy, in one place.</figcaption>
  </div>
  <div class="shot-carousel-nav">
    <button class="shot-carousel-dot active" data-index="0" aria-label="Screen 1"></button>
    <button class="shot-carousel-dot" data-index="1" aria-label="Screen 2"></button>
    <button class="shot-carousel-dot" data-index="2" aria-label="Screen 3"></button>
    <button class="shot-carousel-dot" data-index="3" aria-label="Screen 4"></button>
    <button class="shot-carousel-dot" data-index="4" aria-label="Screen 5"></button>
  </div>
</div>

<script>
(function() {
  var root = document.getElementById('vibe-shot-carousel');
  if (!root) return;
  var slides = root.querySelectorAll('.shot-slide');
  var dots = root.querySelectorAll('.shot-carousel-dot');
  var current = 0;
  var timer;

  function goTo(index) {
    slides[current].classList.remove('active');
    dots[current].classList.remove('active');
    current = (index + slides.length) % slides.length;
    slides[current].classList.add('active');
    dots[current].classList.add('active');
  }

  function startAuto() {
    timer = setInterval(function() { goTo(current + 1); }, 4000);
  }

  dots.forEach(function(dot, i) {
    dot.addEventListener('click', function() {
      clearInterval(timer);
      goTo(i);
      startAuto();
    });
  });

  startAuto();
})();
</script>

---

## **Built to Scale**

For schools and colleges deciding whether to adopt ViBe:

<div class="audience-grid">
  <div class="audience-card">
    <i class="ph ph-lock-open audience-card-icon"></i>
    <div class="audience-card-title">Open-Source, Self-Hostable</div>
    <p class="audience-card-desc">Free to use and free to host yourself. No per-student fees, no lock-in.</p>
  </div>
  <div class="audience-card">
    <i class="ph ph-user-focus audience-card-icon"></i>
    <div class="audience-card-title">Automatic Engagement Enforcement</div>
    <p class="audience-card-desc">If a student stops engaging, ViBe flags and warns them automatically. Students can appeal too, so no manual follow-up is needed.</p>
  </div>
  <div class="audience-card">
    <i class="ph ph-clipboard-text audience-card-icon"></i>
    <div class="audience-card-title">Audit Trail</div>
    <p class="audience-card-desc">Every action taken on the platform is logged, so admins can check what happened and when.</p>
  </div>
  <div class="audience-card">
    <i class="ph ph-user-check audience-card-icon"></i>
    <div class="audience-card-title">Gated Enrollment</div>
    <p class="audience-card-desc">Teachers or admins can approve who joins a course, instead of leaving it open to anyone.</p>
  </div>
  <div class="audience-card">
    <i class="ph ph-flag audience-card-icon"></i>
    <div class="audience-card-title">Proven at National Scale</div>
    <p class="audience-card-desc">Already running as part of a real Ministry of Education programme, not just a test.</p>
  </div>
</div>

---

## **The Impact**

ViBe is already used nationwide as part of the Ministry of Education's Malaviya Mission Teacher Training Programme.

<div class="stat-row">
  <div class="stat"><span class="stat-number">9,984</span><span class="stat-label">Unique Learners</span></div>
  <div class="stat"><span class="stat-number">10,959</span><span class="stat-label">Active Enrollments</span></div>
  <div class="stat"><span class="stat-number">39</span><span class="stat-label">Courses & Cohorts Live</span></div>
  <div class="stat"><span class="stat-number">~35%</span><span class="stat-label">Completion Rate</span></div>
</div>

Most self-paced online courses see under 10% of learners finish. ViBe gets 3.5 times that, with real proctoring, at a very low cost per learner.

Built at the VLED Lab, IIT Ropar, with support from UGC.

---

## **Learner Feedback**

<div class="split-media">
<p>What does it feel like to learn on ViBe? Here is a glimpse from the platform.</p>

{% include video-thumb.html id="AWuA4b9dUpM" title="ViBe – Learner Feedback" %}
</div>

---

Experience the rhythm of learning today at [vibe.vicharanashala.ai](https://vibe.vicharanashala.ai){:target="_blank"}.
