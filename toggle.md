```js

jQuery(document).ready(function(){
	
	jQuery(".games-toggle-btn img").click(function(){
		jQuery(".toggle-game-card").toggleClass("d-none");
		jQuery(".games-toggle-btn").toggleClass("open");
	});
});
