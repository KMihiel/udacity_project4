## Website Performance Optimization portfolio project

To Begin Reviewing my Project please open Index.html in a Web Browser.
	- To test the speed of Index.html run the file through Google's Page Speed Program.
	- To determine FPS of Pizzeria.html please use Chrome Dev Tools Timeline in your Browser 

____________________

My Customizations To Increase WebSpeed 

1.) Compress image size for all jpgs and pngs
	- The key is to compress images file size without compromizing the visual quality 
	- Only shrink physical size when neccesary to prevent stretching pixels
2.) Making unneccesary JS function async
	- Run Google analytic and non-essential JS functions after the page as rendered.
	- This prevents slowing the rendering of the DOM.
3.) Inline styling index.html to increase page load.
	- When styling is minimal it is faster for the DOM if styles are inlined.
4.) Minimize all CSS files.
	- Remove all tabing and white space fro the document
	- This won't assist with sped dramatically but will still help.
5.) Remove variables from inside loops in the JS files
	- Recalling an unchanging variable everytime a loop runs creates unneccesary lag.
	- Declaring variables prior to running the loop prevents repeating code. 
6.) Load only Pizzas that are above the fold to prevent lag. 
	- Painting to the page will add time to FPS, so only paint what is above the fold.
	- Painting unseen images adds unneccesary load time. 
	- Paint what is below the fold only as it required to be visible on the screen.  

Test Code then Optimize, and Always Minify and Cache when possible!
_____________________

### Optimization Tips and Tricks
* [Optimizing Performance](https://developers.google.com/web/fundamentals/performance/ "web performance")
* [Analyzing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/analyzing-crp.html "analyzing crp")
* [Optimizing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/optimizing-critical-rendering-path.html "optimize the crp!")
* [Avoiding Rendering Blocking CSS](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/render-blocking-css.html "render blocking css")
* [Optimizing JavaScript](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/adding-interactivity-with-javascript.html "javascript")
* [Measuring with Navigation Timing](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/measure-crp.html "nav timing api"). We didn't cover the Navigation Timing API in the first two lessons but it's an incredibly useful tool for automated page profiling. I highly recommend reading.
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/eliminate-downloads.html">The fewer the downloads, the better</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/optimize-encoding-and-transfer.html">Reduce the size of text</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/image-optimization.html">Optimize images</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/http-caching.html">HTTP caching</a>