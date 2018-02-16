# Just an example of progress bar animation.

Interview question:
1. If I iterated 10e6 times and on each iteration update width of progress
bar with style.width, would I get smooth updates?
2. If there's a problem with it, how do I make it smooth?

Answer:
1. No, UI will freeze for the duration of loop and then progress bar will be
updated to 100% all at once.
2. You can do it with setTimeout updates or - better - with help of
 requestAnimationFrame.
