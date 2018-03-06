---
layout: default
title: Roger Ehmpke - Web, Graphic and User Interface Designer
description: "Roger Ehmpke, Web, Graphic and User Interface Designer"
keywords: Roger Ehmpke, Web, Web Developer, UI, Front End Developer, Web Designer,
---
<script
  src="http://code.jquery.com/jquery-3.3.1.min.js"
  integrity="sha256-FgpCb/KJQlLNfOu91ta32o/NMZxltwRo8QtmkMRdAu8="
  crossorigin="anonymous"></script>
<script >
  $(document).ready(function() {
    //feed to parse
    var feed = "https://feeds.feedburner.com/raymondcamdensblog?format=xml";
    
    $.ajax(feed, {
        accepts:{
            xml:"application/rss+xml"
        },
        dataType:"xml",
        success:function(data) {
            //Credit: http://stackoverflow.com/questions/10943544/how-to-parse-an-rss-feed-using-javascript

            $(data).find("item").each(function () { // or "item" or whatever suits your feed
                var el = $(this);
                console.log("------------------------");
                console.log("title      : " + el.find("title").text());
                console.log("link       : " + el.find("link").text());
                console.log("description: " + el.find("description").text());
            });
    

        }   
    });
    
});
</script>
<section class="hero-shot">
  <div class="row space-top space-bottom double">
    <div class="column">
      <div class="columns large-4 medium-4">
        <img src="/assets/img/roger.jpg" style="border-radius: 50%;border: 0 solid white;margin:0 auto;"/>
      </div>
      <div class="columns large-8 medium-8">
      <h2>Frontend Web Developer</h2>
      <p>I am a web coordinator currently focusing on the field of frontend web development and JavaScript programming, React, and Redux. My current goal is to obtain either remote web development opportunities and/or part-time/contract employment as a frontend web application developer.</p>
      <p>For over 2 decades I have designed and built portal sites to address design problems. I manage sites in the education industry and have in the nutritional supplement industry as well. I strive to create usable and polished products through passionate and deliberate design.</p>
      <p>I live in Kankakee Illinois. I enjoy music, oil painting, and single malt whiskey.</p>
        <p>Contact me or reach out via LinkedIn or send an email.</p>
      </div>
    </div>
  </div>
</section>
<section id="why">
    <div class="container">
        <div class="row space-top">
          <div class="column">
            <div class="columns large-12 text-center">
                <h2 class="section-heading" style="color:#333333;">About</h2>
                <hr class="primary">
                <br>
            </div>
          </div>
        </div>
    </div>
    <div class="container">
        <div class="row">
          <div class="column">
            <div class="columns large-4 medium-4 text-center">
                <div class="service-box">
                    <i class="fa fa-4x fa-diamond wow bounceIn text-primary" style="color:#fdcc52;"></i>
                    <h3 style="color:#333333;">Ideas</h3>
                    <p class="text-muted">I collaborate with clients and peers to nurture and transform ideas into well thought out design specs. After all, that's where the majority of amazing user experiences start.</p>
                </div>
            </div>
            <div class="columns large-4 medium-4 text-center">
                <div class="service-box">
                    <i class="fa fa-4x fa-magic wow bounceIn text-primary" style="color:#fdcc52;" data-wow-delay=".2s"></i>
                    <h3 style="color:#333333;">UX/UI</h3>
                    <p class="text-muted">I sketch and wireframe interfaces focusing on content structure, intuitive UI patterns and simple interactions. I'm a minimalist who truly believes that less is more.</p>
                </div>
            </div>
                <div class="columns large-4 medium-4 text-center">
                <div class="service-box">
                    <i class="fa fa-4x fa-code wow bounceIn text-primary" style="color:#fdcc52;" data-wow-delay=".3s"></i>
                    <h3 style="color:#333333;">Code</h3>
                    <p class="text-muted"> design in the browser with HTML(5), CSS(3) and a touch of JavaScript. I love coding things from scratch, but I can work with front-end frameworks like Bootstrap too.</p>
                </div>
              </div>
            </div>
        </div>
    </div>
</section>
