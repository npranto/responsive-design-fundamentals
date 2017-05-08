Responsive Design
- abaptibility of content management in varying screen sizes
- designing content with structure, so it is visually appealing and easy to navigate in different devices - mobile, tablet, desktop or others

Hardware Pixels vs Device Independent Pixels
- Hardware pixels refer to the actual physical number of pixels on a device whereas device independent pixels (DIP) is an unit of measurement that relate pixels to actual distance. The browser uses DIP measurement to show different sites in different screen sizes

CSS pixels = device hardware pixels / device independent pixels
i.e., 
	a tablet with width of 640px and dip of 2 would have viewport width of (640/2) = 320px;

In CSS, child elements can overflow the parent container if thier sizes are bigger. In that case, using relative measurements should be implemented
i.e., 
	In the following example, assuming that the img is bigger larger than 300px, it will overflow from the .container div:
		<div class="container" style="width: 300px; height: auto;">
			<img src="https://onehdwallpaper.com/wp-content/uploads/2015/07/Beautiful-Scenery-HD-Wallpapers-Pictures-7.jpg" alt="Beautiful Scenery" />
		</div>
	In these cases, use the following CSS to control the image sizes and to contain within the container div:
		img{
			max-width: 100%;
		}

