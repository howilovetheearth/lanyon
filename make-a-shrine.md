---
layout: page
title: Building a Shrine
url: /make-a-shrine
gallery-root: /assets/images/examples/
display-date: "January 12th, 2021"
---

## Make your own shrine!
It's really simple! Just follow these steps:

1. Identify a public location (we suggest avoiding government offices,
to foreclose any security concerns that our shrines are dangerous).
2. Print out however many messages you want from
<a href="https://drive.google.com/drive/folders/1aRpAN8JHmypNuLKORxiVDTqmN1Rxosm6"
    target="_blank">
    this folder
</a>.
3. Bring tape and consider bringing chalk,
 flowers and candles.
4. Take pictures of your mural (please
<a href="/connect"
    target="_blank">
    send them to us
</a>
), create more murals, share this website with others and stay strong!

## Pictures of Shrines
<div id="gallery">
  {% for image in site.static_files %}
    {% if image.path contains page.gallery-root %}
	<img alt="{{ page.title }}:{{ page.display-date }}" src="{{ image.path }}"
				data-image="{{ image.path }}"
				data-description="{{ page.title }}:{{ page.display-date }}">
	{% endif %}
  {% endfor %}
</div>

<br/>
<script type="text/javascript">
jQuery(document).ready(function(){
    jQuery("#gallery").unitegallery({
        gallery_theme: "tiles",
        tiles_type: "nested",
        tiles_min_columns: 1,
        tiles_nested_optimal_tile_width: 400
    });
});
</script>
