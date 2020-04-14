<!-- ---
id: doc
title: Get Started
sidebar_label: Get Started
--- -->


## Installation
create new app
```js
npm install -g rigel-cli 
```

## Add Files
### screens
```js 
rigel add <screen-name>
```
### components
```js 
rigel add <component-name>
```
### reducers
```js 
rigel add <reducer-name>
```
### saga
```js 
rigel add <saga-name>
```
### actions
```js 
rigel add <action-name>
```
### types
```js 
rigel add <types-name>
```

## Options
### --imc
will view a list of exist components under /App/components, \
select all components you need to import
```js
rigel add Home --imc
```

### --imct
will view a list of exist actions under /App/redux/actions, \
select all actions you need to import
```js
rigel add Home --imct
```

### --export
works with screens, should export the created screen to /App/Navigation/AppNavigation
```js
rigel add Home --export
```

### --connect
create screen with it's own redux files , \
(reducer-types, reducer-action, reducer, reducer-saga, screen, screen-styles), all files works together
```js
rigel add Home --connect
```

### --redux
 create redux files, \
 (reducer-types, reducer-action, reducer, reducer-saga)
 ```js
rigel add Home --redux
```

### --case
take the type case for redux, \
works with reducer, actions, sagas, types, --connect, --redux options
```js
rigel add Home --case=TYPE
```