# api documentation for  react-dnd (v2.3.0)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-dnd.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-dnd) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-dnd.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-dnd)
#### Drag and Drop for React

[![NPM](https://nodei.co/npm/react-dnd.png?downloads=true)](https://www.npmjs.com/package/react-dnd)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-dnd/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-react-dnd_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-dnd/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-dnd/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-dnd/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "dependencies": {
        "disposables": "^1.0.1",
        "dnd-core": "^2.3.0",
        "hoist-non-react-statics": "^1.2.0",
        "invariant": "^2.1.0",
        "lodash": "^4.2.0"
    },
    "description": "Drag and Drop for React",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "aede61c06b968554dcf2a2445657cdbb3100be49",
        "tarball": "https://registry.npmjs.org/react-dnd/-/react-dnd-2.3.0.tgz"
    },
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "darthtrevino",
            "email": "darthtrevino@gmail.com"
        },
        {
            "name": "gaearon",
            "email": "dan.abramov@gmail.com"
        },
        {
            "name": "jordangens",
            "email": "jordangens@gmail.com"
        }
    ],
    "name": "react-dnd",
    "optionalDependencies": {},
    "peerDependencies": {
        "react": "^0.14.0 || ^15.0.0-0"
    },
    "readme": "ERROR: No README data found!",
    "scripts": {
        "babel": "../../node_modules/.bin/babel src --out-dir lib",
        "build": "../../node_modules/.bin/npm-run-all --parallel bundle:* babel",
        "bundle:min": "../../node_modules/.bin/webpack --output-filename=dist/ReactDnD.min.js --optimize-minimize",
        "bundle:unmin": "../../node_modules/.bin/webpack --output-filename=dist/ReactDnD.js",
        "clean": "../../node_modules/.bin/rimraf lib dist",
        "prepublish": "npm test",
        "test": "../../node_modules/.bin/npm-run-all clean build"
    },
    "version": "2.3.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module react-dnd](#apidoc.module.react-dnd)
1.  [function <span class="apidocSignatureSpan">react-dnd.</span>DragDropContext (backendOrModule)](#apidoc.element.react-dnd.DragDropContext)
1.  [function <span class="apidocSignatureSpan">react-dnd.</span>DragDropContextProvider (props, context)](#apidoc.element.react-dnd.DragDropContextProvider)
1.  [function <span class="apidocSignatureSpan">react-dnd.</span>DragLayer (collect)](#apidoc.element.react-dnd.DragLayer)
1.  [function <span class="apidocSignatureSpan">react-dnd.</span>DragSource (type, spec, collect)](#apidoc.element.react-dnd.DragSource)
1.  [function <span class="apidocSignatureSpan">react-dnd.</span>DropTarget (type, spec, collect)](#apidoc.element.react-dnd.DropTarget)
1.  object <span class="apidocSignatureSpan">react-dnd.</span>areOptionsEqual
1.  object <span class="apidocSignatureSpan">react-dnd.</span>createSourceConnector
1.  object <span class="apidocSignatureSpan">react-dnd.</span>createSourceFactory
1.  object <span class="apidocSignatureSpan">react-dnd.</span>createSourceMonitor
1.  object <span class="apidocSignatureSpan">react-dnd.</span>createTargetConnector
1.  object <span class="apidocSignatureSpan">react-dnd.</span>createTargetFactory
1.  object <span class="apidocSignatureSpan">react-dnd.</span>createTargetMonitor
1.  object <span class="apidocSignatureSpan">react-dnd.</span>decorateHandler
1.  object <span class="apidocSignatureSpan">react-dnd.</span>registerSource
1.  object <span class="apidocSignatureSpan">react-dnd.</span>registerTarget
1.  object <span class="apidocSignatureSpan">react-dnd.</span>wrapConnectorHooks

#### [module react-dnd.DragDropContext](#apidoc.module.react-dnd.DragDropContext)
1.  [function <span class="apidocSignatureSpan">react-dnd.DragDropContext.</span>createChildContext (backend, context)](#apidoc.element.react-dnd.DragDropContext.createChildContext)
1.  [function <span class="apidocSignatureSpan">react-dnd.DragDropContext.</span>default (backendOrModule)](#apidoc.element.react-dnd.DragDropContext.default)
1.  [function <span class="apidocSignatureSpan">react-dnd.DragDropContext.</span>unpackBackendForEs5Users (backendOrModule)](#apidoc.element.react-dnd.DragDropContext.unpackBackendForEs5Users)
1.  object <span class="apidocSignatureSpan">react-dnd.DragDropContext.</span>CHILD_CONTEXT_TYPES

#### [module react-dnd.DragDropContextProvider](#apidoc.module.react-dnd.DragDropContextProvider)
1.  [function <span class="apidocSignatureSpan">react-dnd.DragDropContextProvider.</span>default (props, context)](#apidoc.element.react-dnd.DragDropContextProvider.default)

#### [module react-dnd.DragLayer](#apidoc.module.react-dnd.DragLayer)
1.  [function <span class="apidocSignatureSpan">react-dnd.DragLayer.</span>default (collect)](#apidoc.element.react-dnd.DragLayer.default)

#### [module react-dnd.DragSource](#apidoc.module.react-dnd.DragSource)
1.  [function <span class="apidocSignatureSpan">react-dnd.DragSource.</span>default (type, spec, collect)](#apidoc.element.react-dnd.DragSource.default)

#### [module react-dnd.DropTarget](#apidoc.module.react-dnd.DropTarget)
1.  [function <span class="apidocSignatureSpan">react-dnd.DropTarget.</span>default (type, spec, collect)](#apidoc.element.react-dnd.DropTarget.default)

#### [module react-dnd.areOptionsEqual](#apidoc.module.react-dnd.areOptionsEqual)
1.  [function <span class="apidocSignatureSpan">react-dnd.areOptionsEqual.</span>default (nextOptions, currentOptions)](#apidoc.element.react-dnd.areOptionsEqual.default)

#### [module react-dnd.createSourceConnector](#apidoc.module.react-dnd.createSourceConnector)
1.  [function <span class="apidocSignatureSpan">react-dnd.createSourceConnector.</span>default (backend)](#apidoc.element.react-dnd.createSourceConnector.default)

#### [module react-dnd.createSourceFactory](#apidoc.module.react-dnd.createSourceFactory)
1.  [function <span class="apidocSignatureSpan">react-dnd.createSourceFactory.</span>default (spec)](#apidoc.element.react-dnd.createSourceFactory.default)

#### [module react-dnd.createSourceMonitor](#apidoc.module.react-dnd.createSourceMonitor)
1.  [function <span class="apidocSignatureSpan">react-dnd.createSourceMonitor.</span>default (manager)](#apidoc.element.react-dnd.createSourceMonitor.default)

#### [module react-dnd.createTargetConnector](#apidoc.module.react-dnd.createTargetConnector)
1.  [function <span class="apidocSignatureSpan">react-dnd.createTargetConnector.</span>default (backend)](#apidoc.element.react-dnd.createTargetConnector.default)

#### [module react-dnd.createTargetFactory](#apidoc.module.react-dnd.createTargetFactory)
1.  [function <span class="apidocSignatureSpan">react-dnd.createTargetFactory.</span>default (spec)](#apidoc.element.react-dnd.createTargetFactory.default)

#### [module react-dnd.createTargetMonitor](#apidoc.module.react-dnd.createTargetMonitor)
1.  [function <span class="apidocSignatureSpan">react-dnd.createTargetMonitor.</span>default (manager)](#apidoc.element.react-dnd.createTargetMonitor.default)

#### [module react-dnd.decorateHandler](#apidoc.module.react-dnd.decorateHandler)
1.  [function <span class="apidocSignatureSpan">react-dnd.decorateHandler.</span>default (_ref)](#apidoc.element.react-dnd.decorateHandler.default)

#### [module react-dnd.registerSource](#apidoc.module.react-dnd.registerSource)
1.  [function <span class="apidocSignatureSpan">react-dnd.registerSource.</span>default (type, source, manager)](#apidoc.element.react-dnd.registerSource.default)

#### [module react-dnd.registerTarget](#apidoc.module.react-dnd.registerTarget)
1.  [function <span class="apidocSignatureSpan">react-dnd.registerTarget.</span>default (type, target, manager)](#apidoc.element.react-dnd.registerTarget.default)

#### [module react-dnd.wrapConnectorHooks](#apidoc.module.react-dnd.wrapConnectorHooks)
1.  [function <span class="apidocSignatureSpan">react-dnd.wrapConnectorHooks.</span>default (hooks)](#apidoc.element.react-dnd.wrapConnectorHooks.default)



# <a name="apidoc.module.react-dnd"></a>[module react-dnd](#apidoc.module.react-dnd)

#### <a name="apidoc.element.react-dnd.DragDropContext"></a>[function <span class="apidocSignatureSpan">react-dnd.</span>DragDropContext (backendOrModule)](#apidoc.element.react-dnd.DragDropContext)
- description and source-code
```javascript
function DragDropContext(backendOrModule) {
  _checkDecoratorArguments2.default.apply(undefined, ['DragDropContext', 'backend'].concat(Array.prototype.slice.call(arguments))); //
eslint-disable-line prefer-rest-params

  var backend = unpackBackendForEs5Users(backendOrModule);
  var childContext = createChildContext(backend);

  return function decorateContext(DecoratedComponent) {
    var _class, _temp;

    var displayName = DecoratedComponent.displayName || DecoratedComponent.name || 'Component';

    var DragDropContextContainer = (_temp = _class = function (_Component) {
      _inherits(DragDropContextContainer, _Component);

      function DragDropContextContainer() {
        _classCallCheck(this, DragDropContextContainer);

        return _possibleConstructorReturn(this, (DragDropContextContainer.__proto__ || Object.getPrototypeOf(DragDropContextContainer
)).apply(this, arguments));
      }

      _createClass(DragDropContextContainer, [{
        key: 'getDecoratedComponentInstance',
        value: function getDecoratedComponentInstance() {
          (0, _invariant2.default)(this.child, 'In order to access an instance of the decorated component it can ' + 'not be a stateless
 component.');
          return this.child;
        }
      }, {
        key: 'getManager',
        value: function getManager() {
          return childContext.dragDropManager;
        }
      }, {
        key: 'getChildContext',
        value: function getChildContext() {
          return childContext;
        }
      }, {
        key: 'render',
        value: function render() {
          var _this2 = this;

          return _react2.default.createElement(DecoratedComponent, _extends({}, this.props, {
            ref: function ref(child) {
              return _this2.child = child;
            }
          }));
        }
      }]);

      return DragDropContextContainer;
    }(_react.Component), _class.DecoratedComponent = DecoratedComponent, _class.displayName = 'DragDropContext(' + displayName + ')',
_class.childContextTypes = CHILD_CONTEXT_TYPES, _temp);


    return (0, _hoistNonReactStatics2.default)(DragDropContextContainer, DecoratedComponent);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-dnd.DragDropContextProvider"></a>[function <span class="apidocSignatureSpan">react-dnd.</span>DragDropContextProvider (props, context)](#apidoc.element.react-dnd.DragDropContextProvider)
- description and source-code
```javascript
function DragDropContextProvider(props, context) {
  _classCallCheck(this, DragDropContextProvider);

  var _this = _possibleConstructorReturn(this, (DragDropContextProvider.__proto__ || Object.getPrototypeOf(DragDropContextProvider
)).call(this, props, context));

  _this.backend = (0, _DragDropContext.unpackBackendForEs5Users)(props.backend);
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-dnd.DragLayer"></a>[function <span class="apidocSignatureSpan">react-dnd.</span>DragLayer (collect)](#apidoc.element.react-dnd.DragLayer)
- description and source-code
```javascript
function DragLayer(collect) {
  var options = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};

  _checkDecoratorArguments2.default.apply(undefined, ['DragLayer', 'collect[, options]'].concat(Array.prototype.slice.call(arguments
))); // eslint-disable-line prefer-rest-params
  (0, _invariant2.default)(typeof collect === 'function', 'Expected "collect" provided as the first argument to DragLayer ' + 'to
 be a function that collects props to inject into the component. ', 'Instead, received %s. ' + 'Read more: http://react-dnd.github
.io/react-dnd/docs-drag-layer.html', collect);
  (0, _invariant2.default)((0, _isPlainObject2.default)(options), 'Expected "options" provided as the second argument to DragLayer
 to be ' + 'a plain object when specified. ' + 'Instead, received %s. ' + 'Read more: http://react-dnd.github.io/react-dnd/docs-
drag-layer.html', options);

  return function decorateLayer(DecoratedComponent) {
    var _class, _temp;

    var _options$arePropsEqua = options.arePropsEqual,
        arePropsEqual = _options$arePropsEqua === undefined ? _shallowEqualScalar2.default : _options$arePropsEqua;

    var displayName = DecoratedComponent.displayName || DecoratedComponent.name || 'Component';

    var DragLayerContainer = (_temp = _class = function (_Component) {
      _inherits(DragLayerContainer, _Component);

      _createClass(DragLayerContainer, [{
        key: 'getDecoratedComponentInstance',
        value: function getDecoratedComponentInstance() {
          (0, _invariant2.default)(this.child, 'In order to access an instance of the decorated component it can ' + 'not be a stateless
 component.');
          return this.child;
        }
      }, {
        key: 'shouldComponentUpdate',
        value: function shouldComponentUpdate(nextProps, nextState) {
          return !arePropsEqual(nextProps, this.props) || !(0, _shallowEqual2.default)(nextState, this.state);
        }
      }]);

      function DragLayerContainer(props, context) {
        _classCallCheck(this, DragLayerContainer);

        var _this = _possibleConstructorReturn(this, (DragLayerContainer.__proto__ || Object.getPrototypeOf(DragLayerContainer)).
call(this, props));

        _this.handleChange = _this.handleChange.bind(_this);

        _this.manager = context.dragDropManager;
        (0, _invariant2.default)(_typeof(_this.manager) === 'object', 'Could not find the drag and drop manager in the context of
 %s. ' + 'Make sure to wrap the top-level component of your app with DragDropContext. ' + 'Read more: http://react-dnd.github.io
/react-dnd/docs-troubleshooting.html#could-not-find-the-drag-and-drop-manager-in-the-context', displayName, displayName);

        _this.state = _this.getCurrentState();
        return _this;
      }

      _createClass(DragLayerContainer, [{
        key: 'componentDidMount',
        value: function componentDidMount() {
          this.isCurrentlyMounted = true;

          var monitor = this.manager.getMonitor();
          this.unsubscribeFromOffsetChange = monitor.subscribeToOffsetChange(this.handleChange);
          this.unsubscribeFromStateChange = monitor.subscribeToStateChange(this.handleChange);

          this.handleChange();
        }
      }, {
        key: 'componentWillUnmount',
        value: function componentWillUnmount() {
          this.isCurrentlyMounted = false;

          this.unsubscribeFromOffsetChange();
          this.unsubscribeFromStateChange();
        }
      }, {
        key: 'handleChange',
        value: function handleChange() {
          if (!this.isCurrentlyMounted) {
            return;
          }

          var nextState = this.getCurrentState();
          if (!(0, _shallowEqual2.default)(nextState, this.state)) {
            this.setState(nextState);
          }
        }
      }, {
        key: 'getCurrentState',
        value: function getCurrentState() {
          var monitor = this.manager.getMonitor();
          return collect(monitor);
        }
      }, {
        key: 'render',
        value: function render() {
          var _this2 = this; ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-dnd.DragSource"></a>[function <span class="apidocSignatureSpan">react-dnd.</span>DragSource (type, spec, collect)](#apidoc.element.react-dnd.DragSource)
- description and source-code
```javascript
function DragSource(type, spec, collect) {
  var options = arguments.length > 3 && arguments[3] !== undefined ? arguments[3] : {};

  _checkDecoratorArguments2.default.apply(undefined, ['DragSource', 'type, spec, collect[, options]'].concat(Array.prototype.slice
.call(arguments))); // eslint-disable-line prefer-rest-params
  var getType = type;
  if (typeof type !== 'function') {
    (0, _invariant2.default)((0, _isValidType2.default)(type), 'Expected "type" provided as the first argument to DragSource to
be ' + 'a string, or a function that returns a string given the current props. ' + 'Instead, received %s. ' + 'Read more: http://
react-dnd.github.io/react-dnd/docs-drag-source.html', type);
    getType = function getType() {
      return type;
    };
  }
  (0, _invariant2.default)((0, _isPlainObject2.default)(spec), 'Expected "spec" provided as the second argument to DragSource to
 be ' + 'a plain object. Instead, received %s. ' + 'Read more: http://react-dnd.github.io/react-dnd/docs-drag-source.html', spec
);
  var createSource = (0, _createSourceFactory2.default)(spec);
  (0, _invariant2.default)(typeof collect === 'function', 'Expected "collect" provided as the third argument to DragSource to be
 ' + 'a function that returns a plain object of props to inject. ' + 'Instead, received %s. ' + 'Read more: http://react-dnd.github
.io/react-dnd/docs-drag-source.html', collect);
  (0, _invariant2.default)((0, _isPlainObject2.default)(options), 'Expected "options" provided as the fourth argument to DragSource
 to be ' + 'a plain object when specified. ' + 'Instead, received %s. ' + 'Read more: http://react-dnd.github.io/react-dnd/docs-
drag-source.html', collect);

  return function decorateSource(DecoratedComponent) {
    return (0, _decorateHandler2.default)({
      connectBackend: function connectBackend(backend, sourceId) {
        return backend.connectDragSource(sourceId);
      },
      containerDisplayName: 'DragSource',
      createHandler: createSource,
      registerHandler: _registerSource2.default,
      createMonitor: _createSourceMonitor2.default,
      createConnector: _createSourceConnector2.default,
      DecoratedComponent: DecoratedComponent,
      getType: getType,
      collect: collect,
      options: options
    });
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-dnd.DropTarget"></a>[function <span class="apidocSignatureSpan">react-dnd.</span>DropTarget (type, spec, collect)](#apidoc.element.react-dnd.DropTarget)
- description and source-code
```javascript
function DropTarget(type, spec, collect) {
  var options = arguments.length > 3 && arguments[3] !== undefined ? arguments[3] : {};

  _checkDecoratorArguments2.default.apply(undefined, ['DropTarget', 'type, spec, collect[, options]'].concat(Array.prototype.slice
.call(arguments))); // eslint-disable-line prefer-rest-params
  var getType = type;
  if (typeof type !== 'function') {
    (0, _invariant2.default)((0, _isValidType2.default)(type, true), 'Expected "type" provided as the first argument to DropTarget
 to be ' + 'a string, an array of strings, or a function that returns either given ' + 'the current props. Instead, received %s. ' + '
Read more: http://react-dnd.github.io/react-dnd/docs-drop-target.html', type);
    getType = function getType() {
      return type;
    };
  }
  (0, _invariant2.default)((0, _isPlainObject2.default)(spec), 'Expected "spec" provided as the second argument to DropTarget to
 be ' + 'a plain object. Instead, received %s. ' + 'Read more: http://react-dnd.github.io/react-dnd/docs-drop-target.html', spec
);
  var createTarget = (0, _createTargetFactory2.default)(spec);
  (0, _invariant2.default)(typeof collect === 'function', 'Expected "collect" provided as the third argument to DropTarget to be
 ' + 'a function that returns a plain object of props to inject. ' + 'Instead, received %s. ' + 'Read more: http://react-dnd.github
.io/react-dnd/docs-drop-target.html', collect);
  (0, _invariant2.default)((0, _isPlainObject2.default)(options), 'Expected "options" provided as the fourth argument to DropTarget
 to be ' + 'a plain object when specified. ' + 'Instead, received %s. ' + 'Read more: http://react-dnd.github.io/react-dnd/docs-
drop-target.html', collect);

  return function decorateTarget(DecoratedComponent) {
    return (0, _decorateHandler2.default)({
      connectBackend: function connectBackend(backend, targetId) {
        return backend.connectDropTarget(targetId);
      },
      containerDisplayName: 'DropTarget',
      createHandler: createTarget,
      registerHandler: _registerTarget2.default,
      createMonitor: _createTargetMonitor2.default,
      createConnector: _createTargetConnector2.default,
      DecoratedComponent: DecoratedComponent,
      getType: getType,
      collect: collect,
      options: options
    });
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-dnd.DragDropContext"></a>[module react-dnd.DragDropContext](#apidoc.module.react-dnd.DragDropContext)

#### <a name="apidoc.element.react-dnd.DragDropContext.createChildContext"></a>[function <span class="apidocSignatureSpan">react-dnd.DragDropContext.</span>createChildContext (backend, context)](#apidoc.element.react-dnd.DragDropContext.createChildContext)
- description and source-code
```javascript
function createChildContext(backend, context) {
  return {
    dragDropManager: new _dndCore.DragDropManager(backend, context)
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-dnd.DragDropContext.default"></a>[function <span class="apidocSignatureSpan">react-dnd.DragDropContext.</span>default (backendOrModule)](#apidoc.element.react-dnd.DragDropContext.default)
- description and source-code
```javascript
function DragDropContext(backendOrModule) {
  _checkDecoratorArguments2.default.apply(undefined, ['DragDropContext', 'backend'].concat(Array.prototype.slice.call(arguments))); //
eslint-disable-line prefer-rest-params

  var backend = unpackBackendForEs5Users(backendOrModule);
  var childContext = createChildContext(backend);

  return function decorateContext(DecoratedComponent) {
    var _class, _temp;

    var displayName = DecoratedComponent.displayName || DecoratedComponent.name || 'Component';

    var DragDropContextContainer = (_temp = _class = function (_Component) {
      _inherits(DragDropContextContainer, _Component);

      function DragDropContextContainer() {
        _classCallCheck(this, DragDropContextContainer);

        return _possibleConstructorReturn(this, (DragDropContextContainer.__proto__ || Object.getPrototypeOf(DragDropContextContainer
)).apply(this, arguments));
      }

      _createClass(DragDropContextContainer, [{
        key: 'getDecoratedComponentInstance',
        value: function getDecoratedComponentInstance() {
          (0, _invariant2.default)(this.child, 'In order to access an instance of the decorated component it can ' + 'not be a stateless
 component.');
          return this.child;
        }
      }, {
        key: 'getManager',
        value: function getManager() {
          return childContext.dragDropManager;
        }
      }, {
        key: 'getChildContext',
        value: function getChildContext() {
          return childContext;
        }
      }, {
        key: 'render',
        value: function render() {
          var _this2 = this;

          return _react2.default.createElement(DecoratedComponent, _extends({}, this.props, {
            ref: function ref(child) {
              return _this2.child = child;
            }
          }));
        }
      }]);

      return DragDropContextContainer;
    }(_react.Component), _class.DecoratedComponent = DecoratedComponent, _class.displayName = 'DragDropContext(' + displayName + ')',
_class.childContextTypes = CHILD_CONTEXT_TYPES, _temp);


    return (0, _hoistNonReactStatics2.default)(DragDropContextContainer, DecoratedComponent);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-dnd.DragDropContext.unpackBackendForEs5Users"></a>[function <span class="apidocSignatureSpan">react-dnd.DragDropContext.</span>unpackBackendForEs5Users (backendOrModule)](#apidoc.element.react-dnd.DragDropContext.unpackBackendForEs5Users)
- description and source-code
```javascript
function unpackBackendForEs5Users(backendOrModule) {
  // Auto-detect ES6 default export for people still using ES5
  var backend = backendOrModule;
  if ((typeof backend === 'undefined' ? 'undefined' : _typeof(backend)) === 'object' && typeof backend.default === 'function') {
    backend = backend.default;
  }
  (0, _invariant2.default)(typeof backend === 'function', 'Expected the backend to be a function or an ES6 module exporting a default
 function. ' + 'Read more: http://react-dnd.github.io/react-dnd/docs-drag-drop-context.html');
  return backend;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-dnd.DragDropContextProvider"></a>[module react-dnd.DragDropContextProvider](#apidoc.module.react-dnd.DragDropContextProvider)

#### <a name="apidoc.element.react-dnd.DragDropContextProvider.default"></a>[function <span class="apidocSignatureSpan">react-dnd.DragDropContextProvider.</span>default (props, context)](#apidoc.element.react-dnd.DragDropContextProvider.default)
- description and source-code
```javascript
function DragDropContextProvider(props, context) {
  _classCallCheck(this, DragDropContextProvider);

  var _this = _possibleConstructorReturn(this, (DragDropContextProvider.__proto__ || Object.getPrototypeOf(DragDropContextProvider
)).call(this, props, context));

  _this.backend = (0, _DragDropContext.unpackBackendForEs5Users)(props.backend);
  return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-dnd.DragLayer"></a>[module react-dnd.DragLayer](#apidoc.module.react-dnd.DragLayer)

#### <a name="apidoc.element.react-dnd.DragLayer.default"></a>[function <span class="apidocSignatureSpan">react-dnd.DragLayer.</span>default (collect)](#apidoc.element.react-dnd.DragLayer.default)
- description and source-code
```javascript
function DragLayer(collect) {
  var options = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};

  _checkDecoratorArguments2.default.apply(undefined, ['DragLayer', 'collect[, options]'].concat(Array.prototype.slice.call(arguments
))); // eslint-disable-line prefer-rest-params
  (0, _invariant2.default)(typeof collect === 'function', 'Expected "collect" provided as the first argument to DragLayer ' + 'to
 be a function that collects props to inject into the component. ', 'Instead, received %s. ' + 'Read more: http://react-dnd.github
.io/react-dnd/docs-drag-layer.html', collect);
  (0, _invariant2.default)((0, _isPlainObject2.default)(options), 'Expected "options" provided as the second argument to DragLayer
 to be ' + 'a plain object when specified. ' + 'Instead, received %s. ' + 'Read more: http://react-dnd.github.io/react-dnd/docs-
drag-layer.html', options);

  return function decorateLayer(DecoratedComponent) {
    var _class, _temp;

    var _options$arePropsEqua = options.arePropsEqual,
        arePropsEqual = _options$arePropsEqua === undefined ? _shallowEqualScalar2.default : _options$arePropsEqua;

    var displayName = DecoratedComponent.displayName || DecoratedComponent.name || 'Component';

    var DragLayerContainer = (_temp = _class = function (_Component) {
      _inherits(DragLayerContainer, _Component);

      _createClass(DragLayerContainer, [{
        key: 'getDecoratedComponentInstance',
        value: function getDecoratedComponentInstance() {
          (0, _invariant2.default)(this.child, 'In order to access an instance of the decorated component it can ' + 'not be a stateless
 component.');
          return this.child;
        }
      }, {
        key: 'shouldComponentUpdate',
        value: function shouldComponentUpdate(nextProps, nextState) {
          return !arePropsEqual(nextProps, this.props) || !(0, _shallowEqual2.default)(nextState, this.state);
        }
      }]);

      function DragLayerContainer(props, context) {
        _classCallCheck(this, DragLayerContainer);

        var _this = _possibleConstructorReturn(this, (DragLayerContainer.__proto__ || Object.getPrototypeOf(DragLayerContainer)).
call(this, props));

        _this.handleChange = _this.handleChange.bind(_this);

        _this.manager = context.dragDropManager;
        (0, _invariant2.default)(_typeof(_this.manager) === 'object', 'Could not find the drag and drop manager in the context of
 %s. ' + 'Make sure to wrap the top-level component of your app with DragDropContext. ' + 'Read more: http://react-dnd.github.io
/react-dnd/docs-troubleshooting.html#could-not-find-the-drag-and-drop-manager-in-the-context', displayName, displayName);

        _this.state = _this.getCurrentState();
        return _this;
      }

      _createClass(DragLayerContainer, [{
        key: 'componentDidMount',
        value: function componentDidMount() {
          this.isCurrentlyMounted = true;

          var monitor = this.manager.getMonitor();
          this.unsubscribeFromOffsetChange = monitor.subscribeToOffsetChange(this.handleChange);
          this.unsubscribeFromStateChange = monitor.subscribeToStateChange(this.handleChange);

          this.handleChange();
        }
      }, {
        key: 'componentWillUnmount',
        value: function componentWillUnmount() {
          this.isCurrentlyMounted = false;

          this.unsubscribeFromOffsetChange();
          this.unsubscribeFromStateChange();
        }
      }, {
        key: 'handleChange',
        value: function handleChange() {
          if (!this.isCurrentlyMounted) {
            return;
          }

          var nextState = this.getCurrentState();
          if (!(0, _shallowEqual2.default)(nextState, this.state)) {
            this.setState(nextState);
          }
        }
      }, {
        key: 'getCurrentState',
        value: function getCurrentState() {
          var monitor = this.manager.getMonitor();
          return collect(monitor);
        }
      }, {
        key: 'render',
        value: function render() {
          var _this2 = this; ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-dnd.DragSource"></a>[module react-dnd.DragSource](#apidoc.module.react-dnd.DragSource)

#### <a name="apidoc.element.react-dnd.DragSource.default"></a>[function <span class="apidocSignatureSpan">react-dnd.DragSource.</span>default (type, spec, collect)](#apidoc.element.react-dnd.DragSource.default)
- description and source-code
```javascript
function DragSource(type, spec, collect) {
  var options = arguments.length > 3 && arguments[3] !== undefined ? arguments[3] : {};

  _checkDecoratorArguments2.default.apply(undefined, ['DragSource', 'type, spec, collect[, options]'].concat(Array.prototype.slice
.call(arguments))); // eslint-disable-line prefer-rest-params
  var getType = type;
  if (typeof type !== 'function') {
    (0, _invariant2.default)((0, _isValidType2.default)(type), 'Expected "type" provided as the first argument to DragSource to
be ' + 'a string, or a function that returns a string given the current props. ' + 'Instead, received %s. ' + 'Read more: http://
react-dnd.github.io/react-dnd/docs-drag-source.html', type);
    getType = function getType() {
      return type;
    };
  }
  (0, _invariant2.default)((0, _isPlainObject2.default)(spec), 'Expected "spec" provided as the second argument to DragSource to
 be ' + 'a plain object. Instead, received %s. ' + 'Read more: http://react-dnd.github.io/react-dnd/docs-drag-source.html', spec
);
  var createSource = (0, _createSourceFactory2.default)(spec);
  (0, _invariant2.default)(typeof collect === 'function', 'Expected "collect" provided as the third argument to DragSource to be
 ' + 'a function that returns a plain object of props to inject. ' + 'Instead, received %s. ' + 'Read more: http://react-dnd.github
.io/react-dnd/docs-drag-source.html', collect);
  (0, _invariant2.default)((0, _isPlainObject2.default)(options), 'Expected "options" provided as the fourth argument to DragSource
 to be ' + 'a plain object when specified. ' + 'Instead, received %s. ' + 'Read more: http://react-dnd.github.io/react-dnd/docs-
drag-source.html', collect);

  return function decorateSource(DecoratedComponent) {
    return (0, _decorateHandler2.default)({
      connectBackend: function connectBackend(backend, sourceId) {
        return backend.connectDragSource(sourceId);
      },
      containerDisplayName: 'DragSource',
      createHandler: createSource,
      registerHandler: _registerSource2.default,
      createMonitor: _createSourceMonitor2.default,
      createConnector: _createSourceConnector2.default,
      DecoratedComponent: DecoratedComponent,
      getType: getType,
      collect: collect,
      options: options
    });
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-dnd.DropTarget"></a>[module react-dnd.DropTarget](#apidoc.module.react-dnd.DropTarget)

#### <a name="apidoc.element.react-dnd.DropTarget.default"></a>[function <span class="apidocSignatureSpan">react-dnd.DropTarget.</span>default (type, spec, collect)](#apidoc.element.react-dnd.DropTarget.default)
- description and source-code
```javascript
function DropTarget(type, spec, collect) {
  var options = arguments.length > 3 && arguments[3] !== undefined ? arguments[3] : {};

  _checkDecoratorArguments2.default.apply(undefined, ['DropTarget', 'type, spec, collect[, options]'].concat(Array.prototype.slice
.call(arguments))); // eslint-disable-line prefer-rest-params
  var getType = type;
  if (typeof type !== 'function') {
    (0, _invariant2.default)((0, _isValidType2.default)(type, true), 'Expected "type" provided as the first argument to DropTarget
 to be ' + 'a string, an array of strings, or a function that returns either given ' + 'the current props. Instead, received %s. ' + '
Read more: http://react-dnd.github.io/react-dnd/docs-drop-target.html', type);
    getType = function getType() {
      return type;
    };
  }
  (0, _invariant2.default)((0, _isPlainObject2.default)(spec), 'Expected "spec" provided as the second argument to DropTarget to
 be ' + 'a plain object. Instead, received %s. ' + 'Read more: http://react-dnd.github.io/react-dnd/docs-drop-target.html', spec
);
  var createTarget = (0, _createTargetFactory2.default)(spec);
  (0, _invariant2.default)(typeof collect === 'function', 'Expected "collect" provided as the third argument to DropTarget to be
 ' + 'a function that returns a plain object of props to inject. ' + 'Instead, received %s. ' + 'Read more: http://react-dnd.github
.io/react-dnd/docs-drop-target.html', collect);
  (0, _invariant2.default)((0, _isPlainObject2.default)(options), 'Expected "options" provided as the fourth argument to DropTarget
 to be ' + 'a plain object when specified. ' + 'Instead, received %s. ' + 'Read more: http://react-dnd.github.io/react-dnd/docs-
drop-target.html', collect);

  return function decorateTarget(DecoratedComponent) {
    return (0, _decorateHandler2.default)({
      connectBackend: function connectBackend(backend, targetId) {
        return backend.connectDropTarget(targetId);
      },
      containerDisplayName: 'DropTarget',
      createHandler: createTarget,
      registerHandler: _registerTarget2.default,
      createMonitor: _createTargetMonitor2.default,
      createConnector: _createTargetConnector2.default,
      DecoratedComponent: DecoratedComponent,
      getType: getType,
      collect: collect,
      options: options
    });
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-dnd.areOptionsEqual"></a>[module react-dnd.areOptionsEqual](#apidoc.module.react-dnd.areOptionsEqual)

#### <a name="apidoc.element.react-dnd.areOptionsEqual.default"></a>[function <span class="apidocSignatureSpan">react-dnd.areOptionsEqual.</span>default (nextOptions, currentOptions)](#apidoc.element.react-dnd.areOptionsEqual.default)
- description and source-code
```javascript
function areOptionsEqual(nextOptions, currentOptions) {
  if (currentOptions === nextOptions) {
    return true;
  }

  return currentOptions !== null && nextOptions !== null && (0, _shallowEqual2.default)(currentOptions, nextOptions);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-dnd.createSourceConnector"></a>[module react-dnd.createSourceConnector](#apidoc.module.react-dnd.createSourceConnector)

#### <a name="apidoc.element.react-dnd.createSourceConnector.default"></a>[function <span class="apidocSignatureSpan">react-dnd.createSourceConnector.</span>default (backend)](#apidoc.element.react-dnd.createSourceConnector.default)
- description and source-code
```javascript
function createSourceConnector(backend) {
  var currentHandlerId = void 0;

  var currentDragSourceNode = void 0;
  var currentDragSourceOptions = void 0;
  var disconnectCurrentDragSource = void 0;

  var currentDragPreviewNode = void 0;
  var currentDragPreviewOptions = void 0;
  var disconnectCurrentDragPreview = void 0;

  function reconnectDragSource() {
    if (disconnectCurrentDragSource) {
      disconnectCurrentDragSource();
      disconnectCurrentDragSource = null;
    }

    if (currentHandlerId && currentDragSourceNode) {
      disconnectCurrentDragSource = backend.connectDragSource(currentHandlerId, currentDragSourceNode, currentDragSourceOptions);
    }
  }

  function reconnectDragPreview() {
    if (disconnectCurrentDragPreview) {
      disconnectCurrentDragPreview();
      disconnectCurrentDragPreview = null;
    }

    if (currentHandlerId && currentDragPreviewNode) {
      disconnectCurrentDragPreview = backend.connectDragPreview(currentHandlerId, currentDragPreviewNode, currentDragPreviewOptions
);
    }
  }

  function receiveHandlerId(handlerId) {
    if (handlerId === currentHandlerId) {
      return;
    }

    currentHandlerId = handlerId;
    reconnectDragSource();
    reconnectDragPreview();
  }

  var hooks = (0, _wrapConnectorHooks2.default)({
    dragSource: function connectDragSource(node, options) {
      if (node === currentDragSourceNode && (0, _areOptionsEqual2.default)(options, currentDragSourceOptions)) {
        return;
      }

      currentDragSourceNode = node;
      currentDragSourceOptions = options;

      reconnectDragSource();
    },

    dragPreview: function connectDragPreview(node, options) {
      if (node === currentDragPreviewNode && (0, _areOptionsEqual2.default)(options, currentDragPreviewOptions)) {
        return;
      }

      currentDragPreviewNode = node;
      currentDragPreviewOptions = options;

      reconnectDragPreview();
    }
  });

  return {
    receiveHandlerId: receiveHandlerId,
    hooks: hooks
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-dnd.createSourceFactory"></a>[module react-dnd.createSourceFactory](#apidoc.module.react-dnd.createSourceFactory)

#### <a name="apidoc.element.react-dnd.createSourceFactory.default"></a>[function <span class="apidocSignatureSpan">react-dnd.createSourceFactory.</span>default (spec)](#apidoc.element.react-dnd.createSourceFactory.default)
- description and source-code
```javascript
function createSourceFactory(spec) {
  Object.keys(spec).forEach(function (key) {
    (0, _invariant2.default)(ALLOWED_SPEC_METHODS.indexOf(key) > -1, 'Expected the drag source specification to only have ' + 'some
 of the following keys: %s. ' + 'Instead received a specification with an unexpected "%s" key. ' + 'Read more: http://react-dnd.
github.io/react-dnd/docs-drag-source.html', ALLOWED_SPEC_METHODS.join(', '), key);
    (0, _invariant2.default)(typeof spec[key] === 'function', 'Expected %s in the drag source specification to be a function. ' + '
Instead received a specification with %s: %s. ' + 'Read more: http://react-dnd.github.io/react-dnd/docs-drag-source.html', key,
key, spec[key]);
  });
  REQUIRED_SPEC_METHODS.forEach(function (key) {
    (0, _invariant2.default)(typeof spec[key] === 'function', 'Expected %s in the drag source specification to be a function. ' + '
Instead received a specification with %s: %s. ' + 'Read more: http://react-dnd.github.io/react-dnd/docs-drag-source.html', key,
key, spec[key]);
  });

  var Source = function () {
    function Source(monitor) {
      _classCallCheck(this, Source);

      this.monitor = monitor;
      this.props = null;
      this.component = null;
    }

    _createClass(Source, [{
      key: 'receiveProps',
      value: function receiveProps(props) {
        this.props = props;
      }
    }, {
      key: 'receiveComponent',
      value: function receiveComponent(component) {
        this.component = component;
      }
    }, {
      key: 'canDrag',
      value: function canDrag() {
        if (!spec.canDrag) {
          return true;
        }

        return spec.canDrag(this.props, this.monitor);
      }
    }, {
      key: 'isDragging',
      value: function isDragging(globalMonitor, sourceId) {
        if (!spec.isDragging) {
          return sourceId === globalMonitor.getSourceId();
        }

        return spec.isDragging(this.props, this.monitor);
      }
    }, {
      key: 'beginDrag',
      value: function beginDrag() {
        var item = spec.beginDrag(this.props, this.monitor, this.component);
        if (process.env.NODE_ENV !== 'production') {
          (0, _invariant2.default)((0, _isPlainObject2.default)(item), 'beginDrag() must return a plain object that represents the
 dragged item. ' + 'Instead received %s. ' + 'Read more: http://react-dnd.github.io/react-dnd/docs-drag-source.html', item);
        }
        return item;
      }
    }, {
      key: 'endDrag',
      value: function endDrag() {
        if (!spec.endDrag) {
          return;
        }

        spec.endDrag(this.props, this.monitor, this.component);
      }
    }]);

    return Source;
  }();

  return function createSource(monitor) {
    return new Source(monitor);
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-dnd.createSourceMonitor"></a>[module react-dnd.createSourceMonitor](#apidoc.module.react-dnd.createSourceMonitor)

#### <a name="apidoc.element.react-dnd.createSourceMonitor.default"></a>[function <span class="apidocSignatureSpan">react-dnd.createSourceMonitor.</span>default (manager)](#apidoc.element.react-dnd.createSourceMonitor.default)
- description and source-code
```javascript
function createSourceMonitor(manager) {
  return new SourceMonitor(manager);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-dnd.createTargetConnector"></a>[module react-dnd.createTargetConnector](#apidoc.module.react-dnd.createTargetConnector)

#### <a name="apidoc.element.react-dnd.createTargetConnector.default"></a>[function <span class="apidocSignatureSpan">react-dnd.createTargetConnector.</span>default (backend)](#apidoc.element.react-dnd.createTargetConnector.default)
- description and source-code
```javascript
function createTargetConnector(backend) {
  var currentHandlerId = void 0;

  var currentDropTargetNode = void 0;
  var currentDropTargetOptions = void 0;
  var disconnectCurrentDropTarget = void 0;

  function reconnectDropTarget() {
    if (disconnectCurrentDropTarget) {
      disconnectCurrentDropTarget();
      disconnectCurrentDropTarget = null;
    }

    if (currentHandlerId && currentDropTargetNode) {
      disconnectCurrentDropTarget = backend.connectDropTarget(currentHandlerId, currentDropTargetNode, currentDropTargetOptions);
    }
  }

  function receiveHandlerId(handlerId) {
    if (handlerId === currentHandlerId) {
      return;
    }

    currentHandlerId = handlerId;
    reconnectDropTarget();
  }

  var hooks = (0, _wrapConnectorHooks2.default)({
    dropTarget: function connectDropTarget(node, options) {
      if (node === currentDropTargetNode && (0, _areOptionsEqual2.default)(options, currentDropTargetOptions)) {
        return;
      }

      currentDropTargetNode = node;
      currentDropTargetOptions = options;

      reconnectDropTarget();
    }
  });

  return {
    receiveHandlerId: receiveHandlerId,
    hooks: hooks
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-dnd.createTargetFactory"></a>[module react-dnd.createTargetFactory](#apidoc.module.react-dnd.createTargetFactory)

#### <a name="apidoc.element.react-dnd.createTargetFactory.default"></a>[function <span class="apidocSignatureSpan">react-dnd.createTargetFactory.</span>default (spec)](#apidoc.element.react-dnd.createTargetFactory.default)
- description and source-code
```javascript
function createTargetFactory(spec) {
  Object.keys(spec).forEach(function (key) {
    (0, _invariant2.default)(ALLOWED_SPEC_METHODS.indexOf(key) > -1, 'Expected the drop target specification to only have ' + 'some
 of the following keys: %s. ' + 'Instead received a specification with an unexpected "%s" key. ' + 'Read more: http://react-dnd.
github.io/react-dnd/docs-drop-target.html', ALLOWED_SPEC_METHODS.join(', '), key);
    (0, _invariant2.default)(typeof spec[key] === 'function', 'Expected %s in the drop target specification to be a function. ' + '
Instead received a specification with %s: %s. ' + 'Read more: http://react-dnd.github.io/react-dnd/docs-drop-target.html', key,
key, spec[key]);
  });

  var Target = function () {
    function Target(monitor) {
      _classCallCheck(this, Target);

      this.monitor = monitor;
      this.props = null;
      this.component = null;
    }

    _createClass(Target, [{
      key: 'receiveProps',
      value: function receiveProps(props) {
        this.props = props;
      }
    }, {
      key: 'receiveMonitor',
      value: function receiveMonitor(monitor) {
        this.monitor = monitor;
      }
    }, {
      key: 'receiveComponent',
      value: function receiveComponent(component) {
        this.component = component;
      }
    }, {
      key: 'canDrop',
      value: function canDrop() {
        if (!spec.canDrop) {
          return true;
        }

        return spec.canDrop(this.props, this.monitor);
      }
    }, {
      key: 'hover',
      value: function hover() {
        if (!spec.hover) {
          return;
        }

        spec.hover(this.props, this.monitor, this.component);
      }
    }, {
      key: 'drop',
      value: function drop() {
        if (!spec.drop) {
          return undefined;
        }

        var dropResult = spec.drop(this.props, this.monitor, this.component);
        if (process.env.NODE_ENV !== 'production') {
          (0, _invariant2.default)(typeof dropResult === 'undefined' || (0, _isPlainObject2.default)(dropResult), 'drop() must either
 return undefined, or an object that represents the drop result. ' + 'Instead received %s. ' + 'Read more: http://react-dnd.github
.io/react-dnd/docs-drop-target.html', dropResult);
        }
        return dropResult;
      }
    }]);

    return Target;
  }();

  return function createTarget(monitor) {
    return new Target(monitor);
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-dnd.createTargetMonitor"></a>[module react-dnd.createTargetMonitor](#apidoc.module.react-dnd.createTargetMonitor)

#### <a name="apidoc.element.react-dnd.createTargetMonitor.default"></a>[function <span class="apidocSignatureSpan">react-dnd.createTargetMonitor.</span>default (manager)](#apidoc.element.react-dnd.createTargetMonitor.default)
- description and source-code
```javascript
function createTargetMonitor(manager) {
  return new TargetMonitor(manager);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-dnd.decorateHandler"></a>[module react-dnd.decorateHandler](#apidoc.module.react-dnd.decorateHandler)

#### <a name="apidoc.element.react-dnd.decorateHandler.default"></a>[function <span class="apidocSignatureSpan">react-dnd.decorateHandler.</span>default (_ref)](#apidoc.element.react-dnd.decorateHandler.default)
- description and source-code
```javascript
function decorateHandler(_ref) {
  var _class, _temp;

  var DecoratedComponent = _ref.DecoratedComponent,
      createHandler = _ref.createHandler,
      createMonitor = _ref.createMonitor,
      createConnector = _ref.createConnector,
      registerHandler = _ref.registerHandler,
      containerDisplayName = _ref.containerDisplayName,
      getType = _ref.getType,
      collect = _ref.collect,
      options = _ref.options;
  var _options$arePropsEqua = options.arePropsEqual,
      arePropsEqual = _options$arePropsEqua === undefined ? _shallowEqualScalar2.default : _options$arePropsEqua;

  var displayName = DecoratedComponent.displayName || DecoratedComponent.name || 'Component';

  var DragDropContainer = (_temp = _class = function (_Component) {
    _inherits(DragDropContainer, _Component);

    _createClass(DragDropContainer, [{
      key: 'getHandlerId',
      value: function getHandlerId() {
        return this.handlerId;
      }
    }, {
      key: 'getDecoratedComponentInstance',
      value: function getDecoratedComponentInstance() {
        return this.decoratedComponentInstance;
      }
    }, {
      key: 'shouldComponentUpdate',
      value: function shouldComponentUpdate(nextProps, nextState) {
        return !arePropsEqual(nextProps, this.props) || !(0, _shallowEqual2.default)(nextState, this.state);
      }
    }]);

    function DragDropContainer(props, context) {
      _classCallCheck(this, DragDropContainer);

      var _this = _possibleConstructorReturn(this, (DragDropContainer.__proto__ || Object.getPrototypeOf(DragDropContainer)).call
(this, props, context));

      _this.handleChange = _this.handleChange.bind(_this);
      _this.handleChildRef = _this.handleChildRef.bind(_this);

      (0, _invariant2.default)(_typeof(_this.context.dragDropManager) === 'object', 'Could not find the drag and drop manager in
 the context of %s. ' + 'Make sure to wrap the top-level component of your app with DragDropContext. ' + 'Read more: http://react
-dnd.github.io/react-dnd/docs-troubleshooting.html#could-not-find-the-drag-and-drop-manager-in-the-context', displayName, displayName
);

      _this.manager = _this.context.dragDropManager;
      _this.handlerMonitor = createMonitor(_this.manager);
      _this.handlerConnector = createConnector(_this.manager.getBackend());
      _this.handler = createHandler(_this.handlerMonitor);

      _this.disposable = new _disposables.SerialDisposable();
      _this.receiveProps(props);
      _this.state = _this.getCurrentState();
      _this.dispose();
      return _this;
    }

    _createClass(DragDropContainer, [{
      key: 'componentDidMount',
      value: function componentDidMount() {
        this.isCurrentlyMounted = true;
        this.disposable = new _disposables.SerialDisposable();
        this.currentType = null;
        this.receiveProps(this.props);
        this.handleChange();
      }
    }, {
      key: 'componentWillReceiveProps',
      value: function componentWillReceiveProps(nextProps) {
        if (!arePropsEqual(nextProps, this.props)) {
          this.receiveProps(nextProps);
          this.handleChange();
        }
      }
    }, {
      key: 'componentWillUnmount',
      value: function componentWillUnmount() {
        this.dispose();
        this.isCurrentlyMounted = false;
      }
    }, {
      key: 'receiveProps',
      value: function receiveProps(props) {
        this.handler.receiveProps(props);
        this.receiveType(getType(props));
      }
    }, {
      key: 'receiveType',
      value: function receiveType(type) {
        if (type === this.currentType) {
          return;
        }

        this.currentType = type;

        var _registerHandler = registerHandler(type, this.handler, this.manager),
            handlerId = _registerHandler.handlerId,
            unregister = _registerHandler.unregister;

        this.handlerId = handlerId;
        this.handlerMonitor.receiveHandlerId(handlerId);
        this.handlerConnector.receiveHandlerId(handlerId);

        var globalMonitor = this.manager.getMonitor();
        var unsubscribe = globalMon ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-dnd.registerSource"></a>[module react-dnd.registerSource](#apidoc.module.react-dnd.registerSource)

#### <a name="apidoc.element.react-dnd.registerSource.default"></a>[function <span class="apidocSignatureSpan">react-dnd.registerSource.</span>default (type, source, manager)](#apidoc.element.react-dnd.registerSource.default)
- description and source-code
```javascript
function registerSource(type, source, manager) {
  var registry = manager.getRegistry();
  var sourceId = registry.addSource(type, source);

  function unregisterSource() {
    registry.removeSource(sourceId);
  }

  return {
    handlerId: sourceId,
    unregister: unregisterSource
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-dnd.registerTarget"></a>[module react-dnd.registerTarget](#apidoc.module.react-dnd.registerTarget)

#### <a name="apidoc.element.react-dnd.registerTarget.default"></a>[function <span class="apidocSignatureSpan">react-dnd.registerTarget.</span>default (type, target, manager)](#apidoc.element.react-dnd.registerTarget.default)
- description and source-code
```javascript
function registerTarget(type, target, manager) {
  var registry = manager.getRegistry();
  var targetId = registry.addTarget(type, target);

  function unregisterTarget() {
    registry.removeTarget(targetId);
  }

  return {
    handlerId: targetId,
    unregister: unregisterTarget
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-dnd.wrapConnectorHooks"></a>[module react-dnd.wrapConnectorHooks](#apidoc.module.react-dnd.wrapConnectorHooks)

#### <a name="apidoc.element.react-dnd.wrapConnectorHooks.default"></a>[function <span class="apidocSignatureSpan">react-dnd.wrapConnectorHooks.</span>default (hooks)](#apidoc.element.react-dnd.wrapConnectorHooks.default)
- description and source-code
```javascript
function wrapConnectorHooks(hooks) {
  var wrappedHooks = {};

  Object.keys(hooks).forEach(function (key) {
    var hook = hooks[key];
    var wrappedHook = wrapHookToRecognizeElement(hook);
    wrappedHooks[key] = function () {
      return wrappedHook;
    };
  });

  return wrappedHooks;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
