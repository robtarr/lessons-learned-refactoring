
## Concatenated IIFEs
# ⬇
# Webpack

![](https://cdn.worldvectorlogo.com/logos/webpack.svg) <!-- .element: style="width: 300px;" -->


coolModule.js
```
(function CoolModule() {

  function thingA() {
    // cool stuff
  }

  function thingB() {
    // interesting stuff
  }

  return {
    thingA: thingA,
    thingB: thingB
  };
})();
```


coolModule.js
```
const thingA => () {
  // cool stuff
}

const thingB => () {
  // interesting stuff
}

export {
  thingA: thingA,
  thingB: thingB
};
```

other.js
```
import { thingA, thingB } from './coolModule';
```


## Webpack
- 📄 1 Bundled JS Asset
- ䷖ Code Splitting <!-- .element: class="fragment" -->
- 🙍🏾‍♂️🙍🏾‍♂️ Dependency Management ...kind of ¯\\\_(ツ)_/¯ <!-- .element: class="fragment" -->
- 📦 Easy to use NPM Packages <!-- .element: class="fragment" -->
- 🔌 Plugins <!-- .element: class="fragment" -->
- 😢 Lots of boilerplate <!-- .element: class="fragment" -->


# 300 <!-- .element: style="font-size: 6em;" -->


<!-- .slide: data-background="images/convergence-pollock.jpg" -->


# app.


<!-- .slide: data-background="images/huge-mistake.gif" -->


# Start Small
