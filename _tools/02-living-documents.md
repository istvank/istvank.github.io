---
title: "Living Documents"
permalink: /tools/living-documents/
excerpt: "Living Documents."
modified: 2016-05-20T16:30:00+02:00
---

<link rel="import" href="https://cdn.rawgit.com/download/polymer-cdn/1.2.3/lib/iron-ajax/iron-ajax.html">
<link rel="import" href="https://cdn.rawgit.com/download/polymer-cdn/1.2.3/lib/marked-element/marked-element.html">

<template is="dom-bind" id="app">
<iron-ajax auto="" url="https://raw.githubusercontent.com/learning-layers/LivingDocumentsServer/master/README.md" handle-as="text" last-response="{{readme}}"></iron-ajax>
<marked-element markdown="`Markdown` is _awesome_!">
  <div class="markdown-html"></div>
</marked-element>
</template>
