# Just an example of progress bar animation.

Interview question:
1. If we iterated 10e6 times in a loop and on each iteration updated width of progress
bar with style.width, would we get smooth updates?
2. If there's a problem with it, how do we make it smooth?

Answer:
1. No, UI will freeze for the duration of loop and then progress bar will be
updated to 100% all at once.
2. You can do it with setTimeout updates or - better - with help of
 requestAnimationFrame.
 
To test:
1. `python -m SimpleHTTPServer`
2. Go to [localhost:8000](http://localhost:8000)
