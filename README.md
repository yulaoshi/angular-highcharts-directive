Angular Highcharts Directive
============================

An [angular](http://angularjs.org/) directive that wraps around [highcharts](http://www.highcharts.com).

See the code below for this convenient and modelar integration.

![USing this directive along with some of the code](https://raw.github.com/rootux/angular-highcharts-directive/master/screenshot_sample.png "Using angular highcharts directive")


h2. HTML
```html
<div>
    <chart value="basicAreaChart" type="area" height="400"></chart>
</div>
```

h2. Angular
```javascript
'use strict';

angular.module('chartsExample.controllers', []).controller('MainCtrl', ['$scope', '$http', function($scope, $http) {
    $http.get("charts/basicAreaChart.json").success(function(data) {
        $scope.basicAreaChart = data;
    });
}]);
```


[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/rootux/angular-highcharts-directive/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

