## Website Performance Optimization portfolio project

Your challenge, if you wish to accept it (and we sure hope you will), is to optimize this online portfolio for speed! 
In particular, optimize the critical rendering path and make this page render as quickly as possible by applying the 
techniques you've picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).
You might find the FPS Counter/HUD Display useful in Chrome developer tools described here: [Chrome Dev Tools tips-and-tricks](https://developer.chrome.com/devtools/docs/tips-and-tricks).

Result: A much improved profolio page can be view at: https://tamminhdao.github.io/WebOptimization/

####Part 1: Optimize PageSpeed Insights score for index.html

1. Minify print.css. Add media attribute to link tag
2. Minify and inline style.css
3. Load fonts using the Web Font Loader
4. Optimize profilepic.jpg and pizzeria.jpg
5. Move script tags to the bottom of the file
6. Add async attribute to the analytic script tag

####Part 2: Optimize Frames per Second in pizza.html

1. Change made to function resizePizzas():
    1. Replace querySelector with getElementById
2. Delete 2 functions determineDx() and SizeSwitcher(size) 
3. Rewrite the function changePizzaSizes(size)
4. Change made to function updatePositions():
    1. Take care of var phase outside of for loop to minimize repeatative calculation in the loop body
    2. Replace querySelectorAll with getElementsByClassName
    3. Move var items outside of the function because it only needs to be ran once
    4. Create a variable lenn for items.length
5. Line 518: Reduce the number of sliding pizzas from 200 to 30

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

### Customization with Bootstrap
The portfolio was built on Twitter's <a href="http://getbootstrap.com/">Bootstrap</a> framework. All custom styles are in `dist/css/portfolio.css` in the portfolio repo.

* <a href="http://getbootstrap.com/css/">Bootstrap's CSS Classes</a>
* <a href="http://getbootstrap.com/components/">Bootstrap's Components</a>
