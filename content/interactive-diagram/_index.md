---
title: Hosted Page vs Form Overview
---

<h1>Hosted Page vs Form Overview</h1>

<div id="interactive_diagram">

  <h2>Hosted Form</h2>
  <ul class="slideshow">
    <li><img src="/images/interactive-diagram/compare-hosted-form0.jpg" alt="" width="363" height="302"></li>
    <li><img src="/images/interactive-diagram/compare-hosted-form1-static.gif" alt="" width="363" height="302"></li>
    <li><img src="/images/interactive-diagram/compare-hosted-form2-static.gif" alt="" width="363" height="302"></li>
    <li><img src="/images/interactive-diagram/compare-hosted-form3-static.gif" alt="" width="363" height="302"></li>
    <li><img src="/images/interactive-diagram/compare-hosted-form4-static.gif" alt="" width="363" height="302"></li>
  </ul>
  <ul class="interactive">
    <li>Iframed inline into your site so it is seamlessly integrated into your existing design and content management</li>
    <li>Maximum control of content and ability to dynamically control look &amp; feel</li>
    <li>User never leaves your site</li>
    <li>Requires merchant hosting an SSL certificate</li>
  </ul>
  <br class="cr">

  <h2>Hosted Page</h2>
  <ul class="slideshow">
    <li><img src="/images/interactive-diagram/compare-hosted-page0.jpg" alt="" width="363" height="302"></li>
    <li><img src="/images/interactive-diagram/compare-hosted-page1-static.gif" alt="" width="363" height="302"></li>
    <li><img src="/images/interactive-diagram/compare-hosted-page2-static.gif" alt="" width="363" height="302"></li>
  </ul>
  <ul class="interactive">
    <li>Easy setup with all secure pages located on RocketGate's secure servers, encrypted 228bit</li>
    <li>Supports multiple static parent page displays</li>
  </ul>
  <br class="cr">

  <h2>Both Methods</h2>
  <img src="/images/interactive-diagram/compare-both0.jpg" alt="" style="float:right" width="363" height="308">
  <ul>
    <li>Both are PCI compliant solutions where a merchant never has to touch the credit card #s</li>
    <li>Dynamic branding through Cascading Style Sheets (CSS)</li>
    <li>Asynchronus purchase page processing</li>
    <li>Multi-lingual</li>
  </ul>
</div>

<script type="text/javascript">
//<![CDATA[
for(var i = 1; i < 5; i++) {
	tmp = new Image();
	tmp.src = '/images/interactive-diagram/compare-hosted-form' + i + '.gif';
}

for(i = 1; i < 3; i++) {
	tmp = new Image();
	tmp.src = '/images/interactive-diagram/compare-hosted-page' + i + '.gif';
}

$(document).ready(function() {

	var i = 0, $slides = $('.slideshow');

	$('.interactive').each(function() {

		var $ul = $(this), locali = i;

		$ul.find('li').click(function() {
			var $vis_slide = $($slides[locali]).find('li:visible'), newindex = $(this).index() + 1;

			if($vis_slide.index() != newindex) {
				$vis_slide.fadeOut(function() {
					var $img = $(this).find('img'), src = $img.attr('src');
					$img.attr('src', src.replace(/\.gif$/, '-static.gif'));
				});

				$($slides[locali]).find('li:eq(' + (newindex) + ')').fadeIn(function() {
					var $img = $(this).find('img'), src = $img.attr('src');
					$img.attr('src', src.replace(/-static\.gif$/, '.gif'));
				});
			}
		});

		i++;
	});
});
//]]>
</script>

