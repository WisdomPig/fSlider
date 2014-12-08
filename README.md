#fSlider

fSlider是一个轻量级的轮播插件。

##demo

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


