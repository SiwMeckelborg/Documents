---
title: Ordliste 2
description: Ordliste
permalink: ordliste.html
type: glossary
---
<nav>
     <h2>Element navigation</h2>
     <ol id="menu">
        <li><a href="#a">A</a></li>

        <li><a href="#b">B</a></li>
        <li><a href="#c">C</a></li>
        <li><a href="#d">D</a></li>
        <li><a href="#e">E</a></li>
        <li><a href="#f">F</a></li>
        <li>G</li>

        <li><a href="#h">H</a></li>
        <li><a href="#i">I</a></li>
        <li>J</li>
        <li><a href="#k">K</a></li>
        <li><a href="#l">L</a></li>
        <li><a href="#m">M</a></li>

        <li><a href="#n">N</a></li>
        <li><a href="#o">O</a></li>
        <li><a href="#p">P</a></li>
        <li><a href="#q">Q</a></li>
        <li><a href="#r">R</a></li>
        <li><a href="#s">S</a></li>

        <li><a href="#t">T</a></li>
        <li><a href="#u">U</a></li>
        <li><a href="#v">V</a></li>
        <li><a href="#w">W</a></li>
        <li>X</li>
        <li>Y</li>

        <li>Z</li>
</ol>
</nav>

<table>
<thead>

<tr>
<th>Begrep</th>
<th>Beskrivelse</th>
</tr>

</thead>

<tbody>
{% assign gs = site.data.glossary | sort:kv[0] %}
{% for kv in gs %}
<tr> <td>{{ kv[0] }} </td><td> {{ kv[1] }} </td></tr>
{% endfor %}
</tbody>
