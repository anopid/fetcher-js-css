# fetcher-js-css
This library implements a perform  async load of dependencies with JavaScript. It also works for stylesheets.

---
## how to import fetcher-js-css script async
___

```javascript
<script>
function onjs() {
		fetcher.loadScript("url", function () {
			// here you can load other script which depend of 1st one...
			console.log('JS loaded')
		});	
	}
</script>
<script async onload="onjs()" type="text/javascript" src="fetcher-js-css.js" ></script>
```
```bash
npm install fetcher-js-css
```
```javascript
fetcher = require('fetcher-js-css');
fetcher.loadCSS('url to CSS',function () {
            console.log('CSS loaded')
        });
fetcher.loadCSS('url',function () {
            console.log('CSS loaded')
        });				
fetcher.loadScript("url", function () {
		console.log('JS loaded')
	});		
```