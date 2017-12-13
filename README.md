npm install fetcher-js-css

fetcher = require('fetcher-js-css');

fetcher.loadCSS('url to CSS',function () {
            console.log('CSS loaded')
        });
		
fetcher.loadCSS('url',function () {
            // here you can load other css which depend of 1st one...
            console.log('CSS loaded')
        });		
		
fetcher.loadScript("url", function () {
        // here you can load other script which depend of 1st one...
		console.log('JS loaded')
	});		