---
layout: byte
title: Download Blob
type: bytes
tag: [JavaScript, Blob]
description: How to download a blob object.
date: 2016-05-02T00:00:00-00:00
draft: false
---
An example of example of how to download a blob object in JavaScript.

```javascript
var a = document.createElement('a');
document.body.appendChild(a);
a.style.display = 'none';

var blob = new Blob([audio], {type: 'audio/mpeg'});
var url = window.URL.createObjectURL(blob);
a.href = url;
a.download = 'file.mp3';
a.click();
window.URL.revokeObjectURL(url);
```
