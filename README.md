## slide-to-submit
A captcha alternative for preventing spam on forms, while maintaining an easy interface for humans.

<a href="http://kthornbloom.com/slidetosubmit/">View Demo</a>

Simply slide the element to the right to submit the form, similar to unlocking an iOS device. (Slide via a mouse drag, or touch!) If a user mistakenly clicks instead, the sliding element will do a little animation to help suggest what to do.

###Usage
Slide To Submit requires jQuery. Add the plugin after jQuery, and initialize it. You may also call options here.

```
<script src="js/jquery.js"></script>
<script src="js/slide-to-submit.js"></script>
<script>
	$('.slide-submit').slideToSubmit({
		errorText: 'Check required fields', // Shown if fields are invalid & browser doesn't have built-in tooltips
		successText: 'Sent!', // Shown before submitting
		submitDelay: 500, // Delay for showing successText
		graceZone: 100 // Pixels from the right that is accepted as a full side
	});
</script>
```

Add the CSS to the header, or include with your other styles:

```
<link rel="stylesheet" href="css/slide-to-submit.css">
```

Add the slide-submit element at the end of your form:

```
<form>
  <div class="slide-submit">
  	<div class="slide-submit-text">Slide To Submit</div>
  	<div class="slide-submit-thumb">»</div>
  </div>
</form>
```

###Versions

0.1.1 - Added support for HTML5 form validation

0.1.0 - Launch
