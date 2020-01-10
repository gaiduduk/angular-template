# Angular template

## Features
1) Script storing schema
2) Simple receiving page params
3) Auto script loading
4) Material design library

## Example
1) upload template project to your http server
2) create in PROJECT_DIR new folder with your page name(NEW_PAGE_NAME)
3) create file NEW_PAGE_NAME/controller.js
```javascript
controller("NEW_APP_NAME", function ($scope, $routeParams) {
    $scope.buttonLabel = "Button " + ($routeParams.arg1 || "none");
})
```
4) create NEW_APP_NAME/index.html
```html
<md-button class="md-raised md-primary" ng-click="open('helloworld/hello!')">Click {{buttonLabel}}</md-button>
```
5) Open web browser on page:
http://PROJECT_DIR/#!/NEW_APP_NAME/param1