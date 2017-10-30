---
layout: post
title:  "Test Bloop"
date:   2016-02-12 13:46:40
categories: jekyll update gallery
---
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

<style>
/*!
 * baguetteBox.js
 * @author  feimosi
 * @version 1.9.1
 * @url https://github.com/feimosi/baguetteBox.js
 */
#baguetteBox-overlay {
  display: none;
  opacity: 0;
  position: fixed;
  overflow: hidden;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 1000000;
  background-color: #222;
  background-color: rgba(0, 0, 0, 0.8);
  -webkit-transition: opacity .5s ease;
  transition: opacity .5s ease; }
  #baguetteBox-overlay.visible {
    opacity: 1; }
  #baguetteBox-overlay .full-image {
    display: inline-block;
    position: relative;
    width: 100%;
    height: 100%;
    text-align: center; }
    #baguetteBox-overlay .full-image figure {
      display: inline;
      margin: 0;
      height: 100%; }
    #baguetteBox-overlay .full-image img {
      display: inline-block;
      width: auto;
      height: auto;
      max-height: 100%;
      max-width: 100%;
      vertical-align: middle;
      -webkit-box-shadow: 0 0 8px rgba(0, 0, 0, 0.6);
         -moz-box-shadow: 0 0 8px rgba(0, 0, 0, 0.6);
              box-shadow: 0 0 8px rgba(0, 0, 0, 0.6); }
    #baguetteBox-overlay .full-image figcaption {
      display: block;
      position: absolute;
      bottom: 0;
      width: 100%;
      text-align: center;
      line-height: 1.8;
      white-space: normal;
      color: #ccc;
      background-color: #000;
      background-color: rgba(0, 0, 0, 0.6);
      font-family: sans-serif; }
    #baguetteBox-overlay .full-image:before {
      content: "";
      display: inline-block;
      height: 50%;
      width: 1px;
      margin-right: -1px; }

#baguetteBox-slider {
  position: absolute;
  left: 0;
  top: 0;
  height: 100%;
  width: 100%;
  white-space: nowrap;
  -webkit-transition: left .4s ease, -webkit-transform .4s ease;
  transition: left .4s ease, -webkit-transform .4s ease;
  transition: left .4s ease, transform .4s ease;
  transition: left .4s ease, transform .4s ease, -webkit-transform .4s ease, -moz-transform .4s ease; }
  #baguetteBox-slider.bounce-from-right {
    -webkit-animation: bounceFromRight .4s ease-out;
            animation: bounceFromRight .4s ease-out; }
  #baguetteBox-slider.bounce-from-left {
    -webkit-animation: bounceFromLeft .4s ease-out;
            animation: bounceFromLeft .4s ease-out; }

@-webkit-keyframes bounceFromRight {
  0% {
    margin-left: 0; }
  50% {
    margin-left: -30px; }
  100% {
    margin-left: 0; } }

@keyframes bounceFromRight {
  0% {
    margin-left: 0; }
  50% {
    margin-left: -30px; }
  100% {
    margin-left: 0; } }

@-webkit-keyframes bounceFromLeft {
  0% {
    margin-left: 0; }
  50% {
    margin-left: 30px; }
  100% {
    margin-left: 0; } }

@keyframes bounceFromLeft {
  0% {
    margin-left: 0; }
  50% {
    margin-left: 30px; }
  100% {
    margin-left: 0; } }

.baguetteBox-button#next-button, .baguetteBox-button#previous-button {
  top: 50%;
  top: calc(50% - 30px);
  width: 44px;
  height: 60px; }

.baguetteBox-button {
  position: absolute;
  cursor: pointer;
  outline: none;
  padding: 0;
  margin: 0;
  border: 0;
  -moz-border-radius: 15%;
       border-radius: 15%;
  background-color: #323232;
  background-color: rgba(50, 50, 50, 0.5);
  color: #ddd;
  font: 1.6em sans-serif;
  -webkit-transition: background-color .4s ease;
  transition: background-color .4s ease; }
  .baguetteBox-button:focus, .baguetteBox-button:hover {
    background-color: rgba(50, 50, 50, 0.9); }
  .baguetteBox-button#next-button {
    right: 2%; }
  .baguetteBox-button#previous-button {
    left: 2%; }
  .baguetteBox-button#close-button {
    top: 20px;
    right: 2%;
    right: calc(2% + 6px);
    width: 30px;
    height: 30px; }
  .baguetteBox-button svg {
    position: absolute;
    left: 0;
    top: 0; }

/*
    Preloader
    Borrowed from http://tobiasahlin.com/spinkit/
*/
.baguetteBox-spinner {
  width: 40px;
  height: 40px;
  display: inline-block;
  position: absolute;
  top: 50%;
  left: 50%;
  margin-top: -20px;
  margin-left: -20px; }

.baguetteBox-double-bounce1,
.baguetteBox-double-bounce2 {
  width: 100%;
  height: 100%;
  -moz-border-radius: 50%;
       border-radius: 50%;
  background-color: #fff;
  opacity: .6;
  position: absolute;
  top: 0;
  left: 0;
  -webkit-animation: bounce 2s infinite ease-in-out;
          animation: bounce 2s infinite ease-in-out; }

.baguetteBox-double-bounce2 {
  -webkit-animation-delay: -1s;
          animation-delay: -1s; }

@-webkit-keyframes bounce {
  0%, 100% {
    -webkit-transform: scale(0);
            transform: scale(0); }
  50% {
    -webkit-transform: scale(1);
            transform: scale(1); } }

@keyframes bounce {
  0%, 100% {
    -webkit-transform: scale(0);
       -moz-transform: scale(0);
            transform: scale(0); }
  50% {
    -webkit-transform: scale(1);
       -moz-transform: scale(1);
            transform: scale(1); } }

  .gallery {
    margin-bottom: 2.5rem;
  }
  .gallery img {
    width: 160px;
  }
</style>



<div class="baguetteBoxOne gallery">


  <a href="https://feimosi.github.io/baguetteBox.js/img/1-1.jpg" data-caption="Golden Gate derp">
      <img src="https://feimosi.github.io/baguetteBox.js/img/thumbs/1-1.jpg" alt="Golden Gate Bridge">
  </a>
  <a href="https://feimosi.github.io/baguetteBox.js/img/1-2.jpg" title="Midnight City">
      <img src="https://feimosi.github.io/baguetteBox.js/img/thumbs/1-2.jpg" alt="Midnight City">
  </a>
  <a href="https://feimosi.github.io/baguetteBox.js/img/1-3.jpg">
      <img src="https://feimosi.github.io/baguetteBox.js/img/thumbs/1-3.jpg" alt="">
  </a>
  <a href="https://feimosi.github.io/baguetteBox.js/img/1-4.jpg">
      <img src="https://feimosi.github.io/baguetteBox.js/img/thumbs/1-4.jpg" alt="">
  </a>
  <a href="https://feimosi.github.io/baguetteBox.js/img/1-5.jpg">
      <img src="https://feimosi.github.io/baguetteBox.js/img/thumbs/1-5.jpg" alt="">
  </a>
  <a href="https://feimosi.github.io/baguetteBox.js/img/1-6.jpg">
      <img src="https://feimosi.github.io/baguetteBox.js/img/thumbs/1-6.jpg" alt="">
  </a>
  <a href="https://feimosi.github.io/baguetteBox.js/img/1-7.jpg">
      <img src="https://feimosi.github.io/baguetteBox.js/img/thumbs/1-7.jpg" alt="">
  </a>
  <a href="https://feimosi.github.io/baguetteBox.js/img/1-8.jpg">
      <img src="https://feimosi.github.io/baguetteBox.js/img/thumbs/1-8.jpg" alt="">
  </a>
</div>



<div>
  <script src="https://feimosi.github.io/baguetteBox.js/js/baguetteBox.js"></script>
  <script>
    baguetteBox.run('.baguetteBoxOne');
  </script>
</div>


Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll’s dedicated Help repository][jekyll-help].

[jekyll]:      http://jekyllrb.com
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-help]: https://github.com/jekyll/jekyll-help

