# after-effects-lib

Simplified library with easings to use with expressions in after effects.
```
const lib = footage("lib.jsx").sourceData;
fr = 1; //frame number

r = lib.sequenceFrames(timeToFrames(), 0,
	[
		[fr, function(){return lib.slide("easeInOutSine", timeToFrames() - f1, 0, 0, 100, 100, 1.1)}],
	]
);

Math.sin(r * Math.PI/180) * 15;
```

Easing functions from http://robertpenner.com/easing/
https://github.com/danro/jquery-easing/blob/master/jquery.easing.js