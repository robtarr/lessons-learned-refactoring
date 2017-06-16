
# Refactoring

> If we want to be successful software developers, we need to learn how to morph an existing system into a desired new shape.

http://www.methodsandtools.com/archive/mikado.php <!-- .element: style="font-size: .6em;" -->


# Find/Replace

ModelModel ➡ ModalModel


```
return {
  show: show,
  detail: detail,
  update: update
}
```
⬇
```
export {
  show: show,
  detail: detail,
  update: update
}
```


```
export {
  show: show,
  detail: detail,
  update: update
}
```
⬇
```
export {
  show,
  detail,
  update
}
```


https://github.com/cpojer/js-codemod <!-- .element: target="_blank" -->


https://github.com/cpojer/js-codemod/blob/master/transforms/trailing-commas.js <!-- .element: target="_blank" -->


# [astexplorer.net](http://astexplorer.net) <!-- .element: target="_blank" -->


- Adding references to modules
- Swapping Libraries with different APIs


## [Lodash Transform](https://gist.github.com/robtarr/d23ba7e5c68d591a7ffddb3c1e7b4a70) <!-- .element: target="_blank" -->
