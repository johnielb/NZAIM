---
layout: section
title: "Appendix 1: Summary of challenges identified in each technical category"
short_title: 
section_number: 
description: Matrix of build, process and use challenges across algorithm and AI technique categories.
---
# Appendix 1: Summary of challenges identified in each technical ([Section 4](../04-section4/)) category

<style>
.a1 {
  width: 100%;
  border-collapse: collapse;
  line-height: 1.35;
  margin: 1.5rem 0;
}
.a1 th, .a1 td {
  padding: 0.45rem 0.6rem;
  border: 1px solid #c8c8e8;
  vertical-align: middle;
  font-size: 0.875rem;
}
/* Column headers */
.a1 th.col-hdr {
  background: #4747c4;
  color: #fff;
  font-weight: 700;
  text-align: center;
  white-space: nowrap;
}
.a1 th.col-hdr a {
  color: #fff;
  text-decoration: underline;
  text-underline-offset: 3px;
  text-decoration-color: rgba(255,255,255,0.5);
}
/* Row challenge label */
.a1 td.ch {
  background: #1e1b5e;
  color: #fff;
  font-weight: 700;
  width: 26%;
}
/* Section header rows */
.a1 td.sec {
  background: #dde0ff;
  color: #1e1b5e;
  font-weight: 400;
}
/* Cell states */
.a1 td.na  { background: #fff; }
.a1 td.dep { background: #e0e0f8; color: #2a2a80; text-align: center; }
.a1 td.app { background: #cacaee; }
.a1 td.dif { background: #5252b0; color: #fff; text-align: center; }
/* Legend row */
.a1 td.leg { background: #fff; color: #1e1b5e; font-weight: 700; }
.a1 td.leg-na  { background: #fff;      color: #666; text-align: center; }
.a1 td.leg-dep { background: #e0e0f8; color: #2a2a80; text-align: center; }
.a1 td.leg-app { background: #cacaee; color: #2a2a80; text-align: center; }
.a1 td.leg-dif { background: #5252b0; color: #fff;    text-align: center; }
</style>

<table class="a1" style="margin-bottom:0.5rem">
  <tbody>
    <tr>
      <td class="leg"><strong>Legend</strong></td>
      <td class="leg-na">Not applicable</td>
      <td class="leg-dep">Dependent</td>
      <td class="leg-app">Manageable</td>
      <td class="leg-dif">Difficult</td>
    </tr>
  </tbody>
</table>

<table class="a1">
  <thead>
    <tr>
      <th class="col-hdr" style="text-align:left">Challenges</th>
      <th class="col-hdr"><a href="../04-section4/#box-4-1-2">Hand-<br>crafted</a></th>
      <th class="col-hdr"><a href="../04-section4/#box-4-1-3">GDO</a></th>
      <th class="col-hdr"><a href="../04-section4/#box-4-1-6">Supervised</a></th>
      <th class="col-hdr"><a href="../04-section4/#box-4-1-7">Unsupervised</a></th>
      <th class="col-hdr"><a href="../04-section4/#box-4-1-9">Generative</a></th>
    </tr>
  </thead>
  <tbody>
    <!-- BUILD -->
    <tr><td class="sec" colspan="6">Build: Challenges addressed during the design and training (if data-driven) of the system</td></tr>
    <tr>
      <td class="ch">Output-outcome misalignment (proxy mismatch)</td>
      <td class="app"></td><td class="app"></td><td class="app"></td><td class="app"></td><td class="dif"></td>
    </tr>
    <tr>
      <td class="ch">Biased, inequitable or homogeneous outputs</td>
      <td class="dep">Designer responsible</td>
      <td class="dep">Designer responsible</td>
      <td class="app"></td><td class="app"></td><td class="dif"></td>
    </tr>
    <tr>
      <td class="ch">Opacity makes it difficult to understand or review</td>
      <td class="na"></td>
      <td class="dep">Technique dependent</td>
      <td class="dep">Technique dependent</td>
      <td class="dep">Technique dependent</td>
      <td class="dif"></td>
    </tr>
    <tr>
      <td class="ch">Input data accuracy assumed</td>
      <td class="na"></td><td class="na"></td>
      <td class="app"></td><td class="app"></td>
      <td class="dif">Often not known</td>
    </tr>
    <tr>
      <td class="ch">Confounding variables biases outputs</td>
      <td class="na"></td><td class="na"></td>
      <td class="app"></td><td class="app"></td>
      <td class="dif"></td>
    </tr>
    <tr>
      <td class="ch">Value chain hard to interrogate</td>
      <td class="na"></td>
      <td class="na"></td>
      <td class="dep">If pre-trained</td>
      <td class="dep">If pre-trained</td>
      <td class="dif"></td>
    </tr>
    <tr>
      <td class="ch">Problem definition difficult</td>
      <td class="na"></td><td class="app"></td><td class="na"></td>
      <td class="dif">No 'truth'</td>
      <td class="na">Highly generalisable</td>
    </tr>
    <tr>
      <td class="ch">Target(s) accuracy assumed</td>
      <td class="na"></td><td class="na"></td><td class="app"></td>
      <td class="na">No target</td>
      <td class="dif">Often not known</td>
    </tr>
    <tr>
      <td class="ch">Output accuracy isn't validated by design</td>
      <td class="na"></td><td class="na"></td><td class="na"></td><td class="app"></td><td class="dif"></td>
    </tr>
    <!-- PROCESS -->
    <tr><td class="sec" colspan="6">Process: Challenges outside the system's build and use relating to how users and the environment interact with the system.</em></td></tr>
    <tr>
      <td class="ch">Users vulnerable to automation bias</td>
      <td class="app"></td><td class="app"></td><td class="app"></td><td class="app"></td>
      <td class="dif">More active controls needed</td>
    </tr>
    <tr>
      <td class="ch">User hijacking</td>
      <td class="dep">'Game'-able</td>
      <td class="dep">'Game'-able if live</td>
      <td class="dep">'Game'-able</td>
      <td class="dep">'Game'-able</td>
      <td class="dif">Often arbitrary</td>
    </tr>
    <!-- USE -->
    <tr><td class="sec" colspan="6">Use: Challenges that may arise during the operation of the system</td></tr>
    <tr>
      <td class="ch">Concept or data drift</td>
      <td class="app"></td>
      <td class="app"></td><td class="app"></td><td class="app"></td><td class="dif"></td>
    </tr>
    <tr>
      <td class="ch">Compute cost</td>
      <td class="na"></td>
      <td class="dep">If DL</td>
      <td class="dep">If DL</td>
      <td class="dep">If DL</td>
      <td class="dif"></td>
    </tr>
    <tr>
      <td class="ch">Hallucination</td>
      <td class="na"></td><td class="na"></td><td class="na"></td><td class="na"></td>
      <td class="dif"></td>
    </tr>
    <tr>
      <td class="ch">Unauthorised data reuse</td>
      <td class="na"></td>
      <td class="na"></td><td class="na"></td><td class="na"></td><td class="dif"></td>
    </tr>
  </tbody>
</table>
