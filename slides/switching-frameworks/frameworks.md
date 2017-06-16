
# New Framework
 - Performance <!-- .element: class="fragment" -->
 - Flexibility <!-- .element: class="fragment" -->
 - Trends <!-- .element: class="fragment" -->
 - Client Demands <!-- .element: class="fragment" -->
 - Ecosystem <!-- .element: class="fragment" -->
 - Personal Preference <!-- .element: class="fragment" -->


<!-- .slide: data-background="/images/dandelion.gif" -->


## How do we move to a new framework?


# Use Both


<!-- .slide: data-background="images/turducken.gif" -->


# Pubsub


## Knockout
```
publish('new-data', { rating: this.rating });
```


## React
```
componentDidMount() {
  subscribe('new-data', (data) => {
    this.setState(data);
  });
}
```


<!-- .slide: data-background="images/decomp/0-ProductGrid.png" -->


<!-- .slide: data-background="images/decomp/1-ProductGrid-grid.png" -->


<!-- .slide: data-background="images/decomp/2-ProductGrid-product.png" -->


<!-- .slide: data-background="images/decomp/3-ProductGrid-image.png" -->


<!-- .slide: data-background="images/decomp/4-ProductGrid-new.png" -->


<!-- .slide: data-background="images/decomp/5-ProductGrid-info.png" -->


<!-- .slide: data-background="images/decomp/6-ProductGrid-details.png" -->


<!-- .slide: data-background="images/decomp/7-ProductGrid-compare.png" -->


<!-- .slide: data-background="images/decomp/8-ProductGrid-ratings.png" -->


![](images/decomp/ratings.png)


## Knockout
```
import React from 'react';
import ReactDOM from 'react-dom';

ko.bindingHandlers.react = {
  init: function(element, valueAccessor, bindings) {
    ReactDOM.render(
      React.createElement(eval(valueAccessor()), bindings()),
      element
    );
  }
};
```


## Knockout
```
<div data-bind="{
  react: 'ProductCardRating',
  name: 'product-card-rating',
  params: item
}">
```


![Best Friends](/images/best-friends.gif) <!-- .element: style="width: 100%;" -->
