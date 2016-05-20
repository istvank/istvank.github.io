---
title: "Living Documents"
permalink: /tools/living-documents/
excerpt: "Living Documents."
modified: 2016-05-20T16:30:00+02:00
---

<link rel="import" href="https://rawgit.com/PolymerElements/iron-ajax/master/iron-ajax.html">
<link rel="import" href="https://rawgit.com/PolymerElements/marked-element/master/marked-element.html">

<iron-ajax auto="" url="https://raw.githubusercontent.com/learning-layers/LivingDocumentsServer/master/README.md" handle-as="text" last-response="{{readme}}"></iron-ajax>
<marked-element markdown="{{readme}}">
  <div class="markdown-html"></div>
</marked-element>
