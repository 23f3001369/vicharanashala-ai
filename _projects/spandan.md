---
layout: page
title: Spandan
parent: Products
order: 2
permalink: /projects/spandan/
quote: "Learning is not a spectator sport."
quote_author: "D. Blocher"
---

<div class="product-page-meta">
  <span class="product-page-status">Deployed</span>
  <a href="https://spandan.fun/spandan" target="_blank" rel="noopener" class="product-try-link">Try it now ↗</a>
</div>

<p class="product-page-tagline">Real-time classroom engagement — the lecture is heard, questions are generated, and the teacher decides what students see.</p>

<div class="product-page-section">
  <h2>The Problem</h2>
  <p>In live classrooms — online or physical — there is no reliable way to know if students are following along while teaching is happening. Traditional tools like polls or quizzes break the flow: they need to be prepared in advance, demand extra attention from an instructor already managing an entire room, and fail to adapt to what is actually being taught at that moment.</p>
</div>

<div class="product-page-section">
  <h2>What We Built</h2>
  <p>Spandan listens to the instructor's live speech, transcribes it, and generates questions grounded in exactly what was just said. The teacher sees them first — approving or discarding before anything goes out. Students respond on their phones, and the room sees results and a live leaderboard update in real time, while the class is still in session.</p>

  <div class="sdl-wrap fade-up">
    <div class="sdl-bar">
      <span class="sdl-dot"></span>
      <span class="sdl-bar-label">Session Live</span>
      <span class="sdl-bar-status" id="sdl-status">Listening</span>
    </div>
    <div class="sdl-cols">
      <div class="sdl-left">
        <div class="sdl-waveform">
          <span class="sdl-wb"></span><span class="sdl-wb"></span><span class="sdl-wb"></span>
          <span class="sdl-wb"></span><span class="sdl-wb"></span><span class="sdl-wb"></span>
          <span class="sdl-wb"></span>
        </div>
        <div class="sdl-transcript" id="sdl-tx"><span class="sdl-cursor">|</span></div>
      </div>
      <div class="sdl-right">
        <div id="sdl-gen">
          <div class="sdl-shimmer-line"></div>
          <div class="sdl-shimmer-line sdl-sh2"></div>
          <div class="sdl-gen-note">Generating question...</div>
        </div>
        <div id="sdl-q" style="display:none">
          <div class="sdl-q-badge">Question ready</div>
          <div class="sdl-q-text" id="sdl-qtext"></div>
          <div class="sdl-q-btns">
            <button class="sdl-approve" onclick="sdlApprove()"><i class="ph ph-check"></i> Send to class</button>
            <button class="sdl-skip" onclick="sdlSkip()">Skip</button>
          </div>
        </div>
        <div id="sdl-res" style="display:none">
          <div class="sdl-res-note">24 students responded</div>
          <div>
            <div class="sdl-brow"><span class="sdl-opt">A</span><div class="sdl-track"><div class="sdl-fill" id="sdl-f0"></div></div><span class="sdl-pct" id="sdl-p0"></span></div>
            <div class="sdl-brow"><span class="sdl-opt">B</span><div class="sdl-track"><div class="sdl-fill" id="sdl-f1"></div></div><span class="sdl-pct" id="sdl-p1"></span></div>
            <div class="sdl-brow"><span class="sdl-opt">C</span><div class="sdl-track"><div class="sdl-fill" id="sdl-f2"></div></div><span class="sdl-pct" id="sdl-p2"></span></div>
            <div class="sdl-brow"><span class="sdl-opt">D</span><div class="sdl-track"><div class="sdl-fill" id="sdl-f3"></div></div><span class="sdl-pct" id="sdl-p3"></span></div>
          </div>
          <div class="sdl-lb">
            <div class="sdl-lb-title">Leaderboard</div>
            <div class="sdl-lb-row"><span class="sdl-rank">1</span><span class="sdl-name">Ananya S.</span><span class="sdl-score" id="sdl-sc0"></span></div>
            <div class="sdl-lb-row"><span class="sdl-rank">2</span><span class="sdl-name">Rohan M.</span><span class="sdl-score" id="sdl-sc1"></span></div>
            <div class="sdl-lb-row"><span class="sdl-rank">3</span><span class="sdl-name">Priya K.</span><span class="sdl-score" id="sdl-sc2"></span></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="product-page-section">
  <h2>In the Room</h2>
  <p>Spandan works best in large rooms where one person is teaching many. University lectures, faculty development programmes, structured workshops. In those settings the bigger the group, the quieter the feedback loop. A session ends and the teacher often walks out with no real read on how much of it landed.</p>
  <p>For the teacher, the benefit is live signal during class while there is still time to act on it. The leaderboard adds to that: students see how the room answered collectively, not just their own choice, and that shared view changes the dynamic of the session.</p>
  <p>Each session generates a record of what was asked, when, and how the room responded. Over time this builds into a picture of which parts of a lecture tend to lose people and which explanations hold. The record is about the teaching, not a report on the students.</p>
</div>

<div class="product-page-section">
  <h2>Where It's Going</h2>
  <p>The harder design problem in question generation is specificity. A question drawn from what the teacher said in that session is more useful than one drawn from the general topic. The next version is built to work at the level of claims, finding specific statements the teacher made and writing from those. The approval step stays — what changes is that what reaches that screen is more targeted.</p>
  <p>The next feature on the roadmap is co-hosting. Right now a session has one teacher and one stream. Co-hosting will let multiple instructors run a session together, each contributing to the question pool — relevant for panel sessions, team-taught courses, and faculty development programmes where more than one expert is in the room.</p>
  <p>Underlying both is a research effort the lab is actively running. What makes a question genuinely useful in a live classroom — novel enough to reward attention, precise enough to be tied to this session, difficult enough that it matters whether you were there — is the question the lab is building Spandan around.</p>
</div>

<script>
(function() {
  var txLines = [
    "...the relationship between these two variables becomes clearer when we consider what happens at the boundary. Notice how the behaviour shifts as we approach the threshold—this is the key insight.",
    "So what we're seeing here is a pattern that repeats at every level of abstraction. The underlying mechanism stays the same. What changes is how we interpret the result.",
    "And this is precisely where most implementations diverge. The assumption is that initial conditions are irrelevant. But as we've seen, they determine everything that follows."
  ];
  var qs = [
    "What determines the system's behaviour as it approaches the threshold?",
    "What remains consistent across different levels of abstraction?",
    "Which factor determines everything that follows in the implementation?"
  ];
  var rs = [[54,28,12,6],[18,52,24,6],[42,30,20,8]];
  var scores = [[120,95,85],[215,180,162],[335,265,245]];

  var round = 0, lineIdx = 0, charIdx = 0, displayedLines = [], txTimer, stateTimer, didApprove;

  function el(id) { return document.getElementById(id); }

  function typeChar() {
    var line = txLines[lineIdx];
    if (charIdx <= line.length) {
      var cur = displayedLines.concat([line.slice(0, charIdx)]);
      el('sdl-tx').innerHTML = cur.slice(-3).join('<br>') + '<span class="sdl-cursor">|</span>';
      charIdx++;
      txTimer = setTimeout(typeChar, 32 + Math.random() * 18);
    } else {
      displayedLines.push(line);
      if (displayedLines.length > 2) displayedLines = displayedLines.slice(-2);
      lineIdx = (lineIdx + 1) % txLines.length;
      charIdx = 0;
      txTimer = setTimeout(typeChar, 900);
    }
  }

  function setStatus(t) { el('sdl-status').textContent = t; }

  function showGen() {
    el('sdl-gen').style.display = 'block';
    el('sdl-q').style.display = 'none';
    el('sdl-res').style.display = 'none';
    setStatus('Generating...');
    didApprove = false;
    stateTimer = setTimeout(showQuestion, 2800);
  }

  function showQuestion() {
    el('sdl-gen').style.display = 'none';
    el('sdl-q').style.display = 'block';
    el('sdl-qtext').textContent = qs[round % qs.length];
    setStatus('Question ready');
    stateTimer = setTimeout(function() { if (!didApprove) sdlApprove(); }, 4000);
  }

  window.sdlApprove = function() {
    didApprove = true;
    clearTimeout(stateTimer);
    el('sdl-gen').style.display = 'none';
    el('sdl-q').style.display = 'none';
    el('sdl-res').style.display = 'block';
    setStatus('Sent to 24 students');
    var r = rs[round % rs.length], sc = scores[round % scores.length];
    setTimeout(function() {
      for (var i = 0; i < 4; i++) { el('sdl-f' + i).style.width = r[i] + '%'; el('sdl-p' + i).textContent = r[i] + '%'; }
      for (var j = 0; j < 3; j++) { el('sdl-sc' + j).textContent = sc[j]; }
    }, 80);
    stateTimer = setTimeout(nextRound, 5000);
  };

  window.sdlSkip = function() { clearTimeout(stateTimer); nextRound(); };

  function nextRound() {
    round++;
    for (var i = 0; i < 4; i++) { el('sdl-f' + i).style.width = '0%'; el('sdl-p' + i).textContent = ''; }
    showGen();
  }

  typeChar();
  stateTimer = setTimeout(showQuestion, 2800);
})();
</script>

<a href="https://github.com/vicharanashala/spandan" target="_blank" rel="noopener" class="product-github-card">
  <i class="ph ph-github-logo"></i>
  <span>View source on GitHub ↗</span>
</a>
