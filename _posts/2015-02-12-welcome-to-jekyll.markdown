---
layout: post
title:  "Welcome to Jekyll!"
date:   2015-02-12 13:46:40
categories: jekyll update
---
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:


<div class="lang-ruby" data-lang="ruby">
{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}
</div>



You'll find this post in your `_posts` directory - edit this post and re-build (or run with the `-w` switch) to see your changes!
To add new posts, simply add a file in the `_posts` directory that follows the convention: YYYY-MM-DD-name-of-post.ext.

Jekyll also offers powerful support for code snippets:


<div class="lang-js" data-lang="js">
{% highlight js %}
// toggle the hamburger open and closed states
var removeClass = true;

$(".navbar-toggle").click(function () {
  $(".navbar-toggle").toggleClass('is-active');
  $(".navbar-menu").toggleClass('active-menu');
  removeClass = false;
});
{% endhighlight %}
</div>

Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll's GitHub repo][jekyll-gh].



<div class="lang-scss" data-lang="scss">
{% highlight scss %}
// navbar
.navbar,
.navbar-spacer {  
  box-sizing: border-box;
  padding: 0;
  display: block;
  position: relative;
  z-index: 100;
  width: 100%;
  height: $navbar-height;
  background: $navbar-color;
  z-index: 99;
  border-top: 1px solid $navbar-border;

  @include laptop {
    border-bottom: 1px solid $navbar-border;
  }
}
{% endhighlight %}
</div>



<div class="lang-css" data-lang="css">
{% highlight css %}
.highlight  { 
  @extend %vertical-rhythm;
  border-width: 1px;
  border-style: solid;
  padding: 0;
  overflow-x: auto
}
{% endhighlight %}
</div>


[jekyll-gh]: https://github.com/mojombo/jekyll
[jekyll]:    http://jekyllrb.com


<div class="lang-html" data-lang="html">
{% highlight html %}
<header class="site-header">
  <div class="wrapper">
    <a class="site-title" href="website.com/">BLoop</a>
{% endhighlight %}
</div>



<div class="lang-php" data-lang="php">
{% highlight php %}
<?php elseif ( is_single() ) : ?>
  <?php the_title( '<h1 class="entry-title"><span class="screen-reader-text">Article Title: </span>', '</h1>' ); ?>
  <div class="blog-author-date">
    <span class="blog-date">Posted on <?php echo get_the_date('M j, Y'); ?></span>
    <?php 
      // Post ID info
      $temp_post = get_post($post_id);
      $user_id = $temp_post->post_author;
      $first_name = get_the_author_meta('first_name',$user_id);
      $last_name = get_the_author_meta('last_name',$user_id);
      $full_name = "{$first_name} {$last_name}";
      echo '<span class="blog-author">by ' . $full_name . ' </span>';
    ?>
  </div>
{% endhighlight %}
</div>





Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll’s dedicated Help repository][jekyll-help].

[jekyll]:      http://jekyllrb.com
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-help]: https://github.com/jekyll/jekyll-help

