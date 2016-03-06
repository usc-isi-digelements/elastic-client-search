# elastic-client-search

Element which provides a web component interface to the elasticsearch client search API, and coordinates building and issuing queries using the elastic.js library.  Satellite elements for query, filters, aggregation, sorting, and paging communicate with this element to make changes to the index object, and to receive results from queries that are issued to an elastic server instance.  


## Credit to [ElasticUI](https://github.com/ElasticUI)
This suite of web components is inspired by the angular project ElasticUI:  Many of the ng directives used in that project are mimicked with these web components.


## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install


