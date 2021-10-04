# Peer-graded-Assignment-Getting-and-Cleaning-Data-Course-Project

<!DOCTYPE html>
<html>
<head>
<meta content='IE=edge' http-equiv='X-UA-Compatible'>
<meta content='width=800' name='viewport'>
<title>RPubs - Peer-graded Assignment: Getting and Cleaning Data Course Project</title>
<meta name="csrf-param" content="authenticity_token" />
<meta name="csrf-token" content="/Wf1cK13LmtgkNrm5WasVuz5JaU5sB2oErVNOry2AOSzpOGrJ7UWZHoV5mONhALOOQOGhw8Ws7nDzf24JzknhQ==" />
<link rel="stylesheet" media="all" href="/assets/application-db3d8f9490de0f0058decd5613b51469ee8c3214db95ce7e0bd47355e96429eb.css" />
<link rel="stylesheet" media="all" href="/assets/pub/show-58702f9d9025877672e50953d29b220ea08ef2b5acac46cef96fb9182e555801.css" />
<script src="/assets/application-050918065a747f23455921e989643a0f9050e5da8573c9858fc4266f0ec88af2.js"></script>
<link rel="stylesheet" href="https://use.typekit.net/tzi3tjz.css">
<script>
  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  })(window,document,'script','https://www.google-analytics.com/analytics.js','ga');
  ga('create', 'UA-20375833-3', 'auto', {'allowLinker': true});
  ga('require', 'linker');
  ga('linker:autoLink', ['rstudio.com', 'rstudio.github.io', 'rviews.rstudio.com', 'community.rstudio.com', 'rpubs.rstudio.com', 'environments.rstudio.com', 'rstudio.org', 'dailies.rstudio.com', 'pages.rstudio.com', 'db.rstudio.com', 'solutions.rstudio.com', 'docs.rstudio.com', 'spark.rstudio.com', 'shiny.rstudio.com', 'education.rstudio.com', 'rstudio.cloud', 'shinyapps.io', 'teamadmin.rstudio.com', 'blog.rstudio.com', 'support.rstudio.com'] );
  ga('send', 'pageview');
</script>

</head>
<body class='show-pub show-toolbars'>
<div class='modal' id='login' style='display: none'>
<div class='modal-header'>
<h1>Sign In</h1>
</div>
<div class='modal-body'>
<div class='alert' id='login_message' style='display: none'></div>
<form action="/auth/login" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="/iCC63pwIQrRtmei3zjjQdi4adpUceqOcfiCGLMApeENEdOTVyh7xEYx6iyCJ7SwnM0zxhmJgohhWFkmuK0SSA==" />
<input name='return_url' type='hidden'>
<div class='fieldset'>
<div class='control-group'>
<label class='control-label' for='login_username'>Username or Email</label>
<div class='controls'>
<input class='input-xlarge' id='login_username' name='username' type='text'>
</div>
</div>
<div class='control-group'>
<label class='control-label' for='login_password'>Password</label>
<div class='controls'>
<input class='input-xlarge' id='login_password' name='password' type='password'>
</div>
</div>
<div class='control-group'>
<a href='/auth/passwordhelp' target='_blank'>Forgot your password?</a>
</div>
</div>
</form>


</div>
<div class='modal-footer'>
<button class='btn btn-primary' id='login-modal-submit'>Sign In</button>
<button class='btn' id='login-modal-cancel'>Cancel</button>
</div>
</div>
<div class='navbar-inner' id='pageheader'>
<div id='branding'>
<h1 id='logo'>
<a href='/'><span id='R'>R</span>Pubs
</a>
</h1>
<span id='tagline'>by RStudio</span>
</div>
<div id='identity'>
<div class='btn-group pull-right'>
<a class='btn btn-inverse btn-small dropdown-toggle' data-toggle='dropdown' href='#'>
<img src="https://secure.gravatar.com/avatar/396d681673767a34d78134009351fdb8?s=14" class="gravatar" alt="gravatar" style="width: 14px; height: 14px"/>
&nbsp;ellagfr
<span class='caret'></span>
</a>
<ul class='dropdown-menu'>
<li><a href="/ellagfr">View profile</a></li>
<li><a href="/profile/edit">Edit profile</a></li>
<li><a href="/profile/setpass">Change password</a></li>
<li class='divider'></li>
<li><a onclick="rpubs_logout(); return false;" href="#">Sign out</a></li>
</ul>
</div>
</div>
</div>
<div id='pagebody'>
<div id='payload'>
<iframe src='//rstudio-pubs-static.s3.amazonaws.com/407555_03495ae8d77f4e73a1ff798026d6b174.html'></iframe>
<button class='btn btn-tiny' id='btn-show-toolbars'>
<i class='icon-resize-small'></i>
</button>
</div>
<div class='navbar navbar-fixed-bottom' id='pagefooter'>
<div class='navbar-inner'>
<div class='container-fluid'>
<ul class='nav' id='pubmeta'>
<li id='pubtitle'>
<label>Peer-graded Assignment: Getting and Cleaning Data Course Project</label>
</li>
<li id='pubauthor'>
<a href="https://rpubs.com/ninjazzle">by Nunno Nugroho</a>
</li>
<li id='pubtime'>
<label>
Last updated
<time datetime='2018-07-26T03:54:57+00:00'>about 3 years ago</time>
</label>
</li>
</ul>
<ul class='nav pull-right'>
<li>
<button class='btn btn-small btn-success' id='btn-comments'>
<i class='icon-comment icon-white'></i>
<span id='comment-verb-hide'>
Hide
</span>
Comments
<span id='comment-count'>
(&ndash;)
</span>
</button>
<button class='btn btn-small btn-info' id='btn-share'>
<i class='icon-share icon-white'></i>
Share
</button>
<button class='btn btn-small btn-inverse' id='btn-hide-toolbars'>
Hide Toolbars
</button>
</li>
</ul>
</div>
</div>
</div>
<div class='modal hide' id='modal-share'>
<div class='modal-body'>
<btn class='close' data-dismiss='modal' type='button'>×</btn>
<h2 class='first'>Post on:</h2>
<p>
<a class='btn btn-primary btn-large' href='https://twitter.com/intent/tweet?original_referer=http%3A%2F%2Frpubs.com%2Fninjazzle%2FDS-JHU-3-4-Final&amp;source=tweetbutton&amp;text=Peer-graded%20Assignment%3A%20Getting%20and%20Cleaning%20Data%20Course%20Project&amp;url=http%3A%2F%2Frpubs.com%2Fninjazzle%2FDS-JHU-3-4-Final' onclick='window.open(this.href, &#39;&#39;, &#39;menubar=no,toolbar=no,resizable=yes,scrollbars=yes,height=275,width=660&#39;);return false;'>
Twitter
</a>
<a class='btn btn-primary btn-large' href='https://www.facebook.com/sharer.php?u=http%3A%2F%2Frpubs.com%2Fninjazzle%2FDS-JHU-3-4-Final&amp;t=Peer-graded%20Assignment%3A%20Getting%20and%20Cleaning%20Data%20Course%20Project' onclick='window.open(this.href, &#39;&#39;, &#39;menubar=no,toolbar=no,resizable=yes,scrollbars=yes,height=350,width=660&#39;);return false;'>
Facebook
</a>
<a class='btn btn-primary btn-large' href='https://plus.google.com/share?url=http%3A%2F%2Frpubs.com%2Fninjazzle%2FDS-JHU-3-4-Final' onclick='window.open(this.href, &#39;&#39;, &#39;menubar=no,toolbar=no,resizable=yes,scrollbars=yes,height=600,width=600&#39;);return false;'>
Google+
</a>
</p>
<hr>
<h3>Or copy &amp; paste this link into an email or IM:</h3>
<input onclick='this.select()' readonly='readonly' value='http://rpubs.com/ninjazzle/DS-JHU-3-4-Final'>
</div>
</div>
<script>
  $('#btn-edit').click(function() {
    location.href = "/ninjazzle/407555/edit";
  });
  $('#btn-delete').mouseover(function() {
    $('#btn-delete').removeClass('btn-inverse').addClass('btn-danger');
  });
  $('#btn-delete').mouseout(function() {
    $('#btn-delete').addClass('btn-inverse').removeClass('btn-danger');
  });
  $('#btn-hide-toolbars').click(function() {
    $(document.body).addClass('hide-toolbars');
    $(document.body).removeClass('show-toolbars');
  });
  $('#btn-show-toolbars').click(function() {
    $(document.body).addClass('show-toolbars');
    $(document.body).removeClass('hide-toolbars');
  });
  $('#btn-share').click(function() {
    $('#modal-share').modal().css({
      'margin-left': function () {
        return -($(this).width() / 2);
      }
    });
  });
  $('#btn-comments').click(function() {
    $(document.body).toggleClass('show-comments');
  });
  setInterval(function() {
    // Poll for comment count. Barf.
    var text = $('#dsq-num-posts').text();
    if (text && /^\d+$/.test(text))
      $('#comment-count').text('(' + text + ')');
  }, 1000);
</script>
<div id='comment-wrapper'>
<div id='disqus_thread'>
<script>
  var disqus_config = function () {
      // The generated payload which authenticates users with Disqus
      this.page.remote_auth_s3 = 'eyJpZCI6InJwdWJzLTM2NDIzNSIsInVzZXJuYW1lIjoiZWxsYWdmciIsImVtYWlsIjoiYmxvbXN0ZWVyZmVAZ21haWwuY29tIiwiYXZhdGFyIjoiaHR0cHM6Ly9zZWN1cmUuZ3JhdmF0YXIuY29tL2F2YXRhci8zOTZkNjgxNjczNzY3YTM0ZDc4MTM0MDA5MzUxZmRiOD9zPTY0IiwidXJsIjoiIn0= be0fb2db7986a501b40f473ee83d99fc3b998f1a 1633313841';
      this.page.author_s3 = 'eyJ1c2VybmFtZSI6InJwdWJzLTE0MjM1MyJ9 62ddd60091fc1a44c8f4f7c7e095771456c4afcc 1633313841';
      this.page.api_key = '7NhtlDm2Hf3z44e8I6PRkOLIwe9o1U0rVepc4PMzqwnADLCB3JhMdX7ZUPbnl85p';
  };
</script>
<script>
  var disqus_shortname = 'rpubs'; // required: replace example with your forum shortname
  var disqus_identifier = 'pub-407555';
  var disqus_developer = 1;
  
  /* * * DON'T EDIT BELOW THIS LINE * * */
  (function() {
    var dsq = document.createElement('script'); dsq.type = 'text/javascript'; dsq.async = true;
    dsq.src = '//' + disqus_shortname + '.disqus.com/embed.js';
    (document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(dsq);
  })();
</script>
</div>
</div>

</div>
</body>
</html>
