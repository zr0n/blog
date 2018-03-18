---
layout: page
title: Input Manager for UE4
---

<p class="message">
  An easy to use UE4 open source plugin to reassign your actions and axis at Runtime. 
</p>

## Instalation

[Download the plugin here](https://github.com/zr0n/UEInputManager/releases/download/1.0/InputManager.zip), then extract the content to your engine or project plugins folder. 
* Re-open your UE4 Editor and enable the Input Manager plugin in Edit > Plugins 

## Possible Failures

* If the editor alert the plugin is not compatible with your version and ask you about disable it, click no and the editor will try to recompile the plugin
* If the previous process still failing, go to your project directory, right click on YourProject.uproject (generally an UE blue logo) and select Generate Visual Studio Files.
* If it still fails, make sure you have all the UE4 build requirements. Maybe this link can help: <a href="https://docs.unrealengine.com/en-us/Programming/Development/VisualStudioSetup"> https://docs.unrealengine.com/en-us/Programming/Development/VisualStudioSetup</a>

## Usage
<blockquote class="imgur-embed-pub" lang="en" data-id="a/Flk3f"><a href="//imgur.com/Flk3f"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

<p class="message"> Use the functions of the image above to <b>look for/reassign</b> input bindings </p>


## Demo

If you want to see the plugin running watch the video below and/or download the example project: <a href="https://goo.gl/LBdbLK">https://goo.gl/LBdbLK</a>
<div class="videoWrapper">
  <iframe width="854" height="480" src="https://www.youtube.com/embed/TAq8prjIXAo" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

## Contribution

If you are a programmer feel free to contribute to the plugin and make the community a better place.

<div id="disqus_thread"></div>
<script>

/**
*  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
*  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables*/
/*
var disqus_config = function () {
this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
};
*/
(function() { // DON'T EDIT BELOW THIS LINE
var d = document, s = d.createElement('script');
s.src = 'https://luiz-fernando.disqus.com/embed.js';
s.setAttribute('data-timestamp', +new Date());
(d.head || d.body).appendChild(s);
})();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
                            