## Angular.js
 * Build SPA application
 * MVVM mode
 * Created by Misko Hevery in 2009
 * Open source , supported by Goggle 
 * [lib link](https://code.angularjs.org/)

## Concepts for Angular.js
 # Bootstrap 
   * auto init --- use ng-app directive 
   * init by manual -- angular.bootstrap(document, ['**moduleName**']);
   * notes -- ng-app and angular.bootstrap can't be used together.
 # Data binding
   * ng-mode + {{}} expressions or ng-mode + ng-bind 
   * one-time binding  {{:: message}} only apply value change one time when the model value changes.
   * two way binding  {{ message }}
 # Controller 
   * register a controller with our angular module
     -- app.module('myModule', []).controler('ControllerName', function(){});
