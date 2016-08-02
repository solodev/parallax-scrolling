# Parallax Scrolling
A major trend in web design is parallax scrolling, which involves the background moving at a slower rate to the foreground thus creating a 3D effect as you scroll down the page. [Solodev](https://www.solodev.com/) shows how to incorporate this subtle element of depth to the background images of your web pages.

## Tutorial

For detailed instructions, view Solodev's [Using Parallax Scrolling with Background Images](https://www.solodev.com/blog/web-design/using-parallax-scrolling-with-background-images.stml) article.

## Demo

Check out a working example on [JSFiddle](http://jsfiddle.net/solodev/7tf7pLb0/).

## HTML

The given section can be created using the following HTML markup:
```
<header class="black-circle parallax" style="min-height: 979px;">
	<div class="inner">
		<div class="ct-page_title">
			<div class="inner">
				<h1>
					<span><img src="images/logo.png"/></span>
				</h1>
				<h2>
					A major trend in web design is parallax scrolling, which involves the background moving at a slower rate to the foreground, creating a 3D effect as you scroll down the page.
				</h2>
			</div>
		</div>
	</div>
</header>
```

## CSS

All CSS is included in parallax.css.

## JavaScript

The background images for each section needs to be initialized with parallax:
```
$(document).ready(function() {
	$('header').parallax({
		imageSrc: 'images/background-1.jpg'
	});

	$('#section2').parallax({
		imageSrc: 'images/background-3.jpg'
	});
});
```

The principle parallax resource, "parallax.min.js" was created by [Pixelcog](https://github.com/pixelcog/parallax.js).

## External Includes

The following third-party resources are needed:
```
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.5.0/css/font-awesome.min.css">
	
<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
<script type="text/javascript" src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
<script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/parallax.js/1.3.1/parallax.min.js"></script>
```

The "font-awesome.min.css" and "bootstrap.min.js" resources are optional depending on the layout and content of your page.