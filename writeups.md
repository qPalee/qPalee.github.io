---
title: Writeups
layout: home
permalink: /writeups/
---

<div>
  <table>
    <thead>
      <td>Challenge</td>
      <td>CTF</td>
    </thead>
    {% for writeup in site.writeups reversed %}
    <tr>
      <td>
        <a href="{{ writeup.url | prepend: site.baseurl }}"> {{ writeup.title }} </a>
      </td>
      <td>
        {{ writeup.ctf }}
      </td>
    </tr>
    {% endfor %}
  </table>
</div>
