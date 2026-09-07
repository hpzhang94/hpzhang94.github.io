---
title: Team
layout: page
permalink: /team/
hide_title: true
---

<!--
  CSS styles for the lab team roster: a responsive two-column grid of
  member cards, each with a floated headshot and a list of degrees.
-->
<style>
  .team-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 1.5em 2.5em;
    margin-bottom: 2em;
  }
  .team-member {
    overflow: hidden;
  }
  /* Square crop + 50% radius so portraits of any aspect ratio render as circles. */
  .team-member img {
    float: left;
    width: 110px;
    height: 110px;
    object-fit: cover;
    margin: 0.2em 1.2em 0.6em 0;
    border-radius: 50%;
  }
  /* The lone faculty card sits centered rather than stretched across the page. */
  .team-grid--faculty {
    display: flex;
    justify-content: center;
  }
  /* Explicit width, not just a cap: the floated headshot is out of flow, so the
     card would otherwise shrink-wrap to the text and squeeze the degree line.
     max-width keeps it from overflowing narrow screens, where it wraps instead. */
  .team-grid--faculty .team-member {
    width: 36em;
    max-width: 100%;
  }
  .team-member h3,
  .team-member h4 {
    margin: 0 0 0.15em 0;
    color: #006994; /* Matches $linkcolor, so linked and plain names agree */
  }
  .team-member .team-role {
    display: block;
    margin: 0 0 0.4em 0;
    font-style: italic;
    color: #6b6b6b;
  }
  .team-member ul {
    overflow: hidden;
    margin: 0;
    padding-left: 1.2em;
  }
  .team-member ul li {
    margin-bottom: 0.2em;
    line-height: 1.4;
  }
</style>

## Faculty

<div class="team-grid team-grid--faculty">

  <div class="team-member">
    <img src="{{ site.github.url }}/images/teampic/Haopeng.png" alt="Haopeng Zhang">
    <h3><a href="https://hpzhang94.github.io/">Haopeng Zhang</a>, Ph.D.</h3>
    <span class="team-role">Assistant Professor</span>
    <ul>
      <li>Ph.D., Computer Science, University of California, Davis</li>
    </ul>
  </div>

</div>

## Members

<div class="team-grid">

  <div class="team-member">
    <img src="{{ site.github.url }}/images/teampic/july.jpg" alt="July Zhang">
    <h4><a href="https://www.instagram.com/qiyuestarla/" target="_blank">July Zhang</a></h4>
    <span class="team-role">honored member</span>
    <ul>
      <li>University of Cute Cat (UCC)</li>
    </ul>
  </div>

  <div class="team-member">
    <img src="{{ site.github.url }}/images/teampic/haohan.jpeg" alt="Haohan Yuan">
    <h4><a href="https://haohanyuan01.github.io/" target="_blank">Haohan Yuan</a></h4>
    <span class="team-role">Ph.D. student (Fall 2024 - )</span>
    <ul>
      <li>M.E. Nanyang Technological University</li>
      <li>B.S. Hefei University of Technology</li>
    </ul>
  </div>

  <div class="team-member">
    <img src="{{ site.github.url }}/images/teampic/cade.jpg" alt="Cade Kane">
    <h4>Cade Kane</h4>
    <span class="team-role">Ph.D. student (Fall 2025 - )</span>
    <ul>
      <li>B.S. University of Hawaii at Manoa</li>
    </ul>
  </div>

  <div class="team-member">
    <img src="{{ site.github.url }}/images/teampic/mengqi.jpeg" alt="Mengqi Shi">
    <h4><a href="https://www.linkedin.com/in/mengqi-shi-60a6a937b/" target="_blank">Mengqi Shi</a></h4>
    <span class="team-role">Ph.D. student (Fall 2025 - )</span>
    <ul>
      <li>M.S. Nanyang Technological University</li>
      <li>B.S. Southeast University</li>
    </ul>
  </div>

  <div class="team-member">
    <img src="{{ site.github.url }}/images/teampic/shouju.jpeg" alt="Shouju Wang">
    <h4><a href="https://www.linkedin.com/in/shouju-wang-4b030a385/" target="_blank">Shouju Wang</a></h4>
    <span class="team-role">Ph.D. student (Fall 2025 - )</span>
    <ul>
      <li>B.S. Wuhan University</li>
    </ul>
  </div>

</div>
