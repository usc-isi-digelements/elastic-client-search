# elastic-client-search

A Polymer Element which provides a web component interface to the elasticsearch client search API, and coordinates building and issuing queries using the elastic.js library.  Satellite elements for query, filters, aggregation, sorting, and paging communicate with this element to make changes to the index object, and to receive results from queries that are issued to an elastic server instance.  

### Example
```html
<elastic-client
  config='{"host": "http://localhost:9200"}'
  client="{{esclient}}"
  cluster-status="{{my-status}}">
</elastic-client>

<elastic-client-search
  client="[[esclient]]"
  index="[[myIndex]]"
  query="[[ejsQuery]]"
  aggregations="[]"
  filters="[[ejsFilters]]"
  results="{{queryResults}}"
  result-count="{{resultCount}}"
  last-error="{{queryError}}"
  loading="{{loading}}">
</elastic-client-search>
```

### Dependencies

Dependencies are installed using [Bower](http://bower.io/):

    npm install -g bower
    bower install

### Testing

Tests require a local instance of elasticsearch with the `mockads` index created by running `data/import_test_data.sh`.

Tests are run using [web-component-tester](https://github.com/Polymer/web-component-tester):

    npm install -g web-component-tester
    wct

### Demonstration & Documentation

Demonstration and documentation are viewed using [polyserve](https://github.com/PolymerLabs/polyserve):

    npm install -g polyserve
    polyserve

