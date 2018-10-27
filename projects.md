---
layout: page
title: Projects
description: Recent work by Sergi Xaudiera
permalink: /projects/
---
<aside>Some of the things I've made (and can be seen)</aside>

<div class="container">
  <a href="/numballs/"><img src="/img/20180827_numballs.png" alt="Numballs" class="image">
  <div class="overlay">
    <div class="text">numballs app</div>
  </div></a>
  <div class="caption">numballs app (2012 - 2018)</div>
</div>
<div class="container">
  <a href="/blog/numballs/"><img src="/img/201210_nbaplayersnetwork.png" alt="Blog Numballs" class="image">
  <div class="overlay">
    <div class="text">numballs blog</div>
  </div></a>
  <div class="caption">numballs blog (2012 - 2018)</div>
</div>
<div style="clear: both">
<div class="container">
  <a href="/cop-gencat/"><img src="/img/2017-02-08-congres-govern-digital.jpg" alt="Blog Personal" class="image">
  <div class="overlay">
    <div class="text">CoP Gencat</div>
  </div></a>
  <div class="caption">CoP Gencat (2010 - now)</div>
</div>
<div class="container">
  <a href="/blog/personal/"><img src="/img/200907_teamGFI2.png" alt="Blog Personal" class="image">
  <div class="overlay">
    <div class="text">personal blog</div>
  </div></a>
  <div class="caption">personal blog (2007 - now)</div>
</div>
<div style="clear: both">
<div class="container">
  <a href="/blog/futbol/"><img src="/img/20121203_ajax95.jpeg" alt="Blog Futbol" class="image">
  <div class="overlay">
    <div class="text">futbol blog</div>
  </div></a>
  <div class="caption">futbol blog (2012 - 2013)</div>
</div>

<style>
.container {
  position: relative;
  width: 45%;
  margin-right: 2%;
  margin-bottom: 4%;
  float: left;
}
.image {
  display: block;
  width: 100%;
  height: 260px;
}
@media only screen and (max-width: 800px) {
  .container {
    width: 100%;
  }
  .image {
    height: auto;
  }

}
.overlay {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100%;
  opacity: 0;
  transition: .5s ease;
  background-color: #faf9f5;
}

.container:hover .overlay {
  opacity: 1;
}

.text {
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  text-align: center;
}
.caption {
  text-align: center;
  min-height: 3rem;
  font-size: 0.8rem;
  line-height: 3rem;
  font-family: courier new;
  color: #fff;
  background: #333;
}

</style>