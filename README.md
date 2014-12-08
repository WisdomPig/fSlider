#fSlider

fSlider是一个轻量级的轮播插件。

##demo

###html
	<div id="slider" class="wrapper">
		<ul id="bannerList" class="slider-list clearfix">
			<li class="slider-item">
				<img src="a.jpg" width="1000" height="400">
			</li>
			<li class="slider-item">
				<img src="b.jpg" width="1000" height="400">
			</li>
			<li class="slider-item">
				<img src="c.jpg" width="1000" height="400">
			</li>
			<li class="slider-item">
				<img src="d.jpg" width="1000" height="400">
			</li>
		</ul>
		<ul id="ctrl" class="btn-list">
			<li class="btn-item">1</li>
			<li class="btn-item">2</li>
			<li class="btn-item">3</li>
			<li class="btn-item">4</li>
		</ul>
	</div>
	<a id="prevItem" class="arrow" href="javascript:;"></a>
	<a id="nextItem" class="arrow" href="javascript:;"></a>

###css
	.wrapper {position: relative;overflow: hidden;}
	.slider-list {position: absolute;height: 100%;top: 0;left: 0;}
	.slider-item {float: left;height: 100%;}

###javascript
	var slider = new Slider($('#slider'), {
		time: 5000,
		delay: 400,
		event: 'hover',
		auto: true,
		mode: 'fade',
		controller: $('#ctrl'),
		activeControllerCls: 'active'
	});

	$('#prevItem').click(function() {
		slider.prev();
	});

	$('#nextItem').click(function() {
		slider.next();
	});


