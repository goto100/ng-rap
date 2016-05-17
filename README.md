

## 安装

* `$ bower install ng-rap`

## 使用

```
angular.module('myApp', ['ngRap']).config(['$httpProvider', 'ngRapProvider', function(httpProvider, ngRapProvider) {
	ngRapProvider.script = 'http://xxx.xxx.xxx/rap.plugin.js?projectId=nnn'; // replce your host and project id
	ngRapProvider.enable({
		mode: 3
	});
	httpProvider.interceptors.push('rapMockInterceptor');
}]);
```
