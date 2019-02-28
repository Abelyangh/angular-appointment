# Angular.js
 * Build SPA application
 * MVVM mode
 * Created by Misko Hevery in 2009
 * Open source , supported by Goggle 
 * [lib link](https://code.angularjs.org/)

## Concepts for Angular.js
 ### Bootstrap 
   * auto init --- use ng-app directive 
   * init by manual -- angular.bootstrap(document, ['**moduleName**']);
   * notes -- ng-app and angular.bootstrap can't be used together.
 ### Data binding
   * ng-mode + {{}} expressions or ng-mode + ng-bind 
   * one-time binding  {{:: message}}
   * two way binding  {{ message }}
 ### Controller 
   * register controller with angular module 
   angular.module('moduleName', []).controller('controllerName', function() {}); 
   * $scope 
   `angular.module('moduleName',[]).controller('appController', function($scope) {
        $scope.message = "***";
    });
      <div ng-controller="appController">
         <span>{{ message }}</span>
      </div>`
   * controller as syntax after version 1.2
      `ng-controller = "appController as ctrl"
       angular.module('app', []).controller('appController', function() {
         var ctrl = this;  //important
       });`
   