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

- will create new dir under screens with the screen name & styles

```js
rigel add screen <screen-name>
```

### components

- will create new dir under components with the component name & styles

```js
rigel add component <component-name>
```

### Slices

- please refer to @redux-toolkit

```js
rigel add slice <name>
```

### API

- Required options dir, url
- Default method is get

```js
rigel add api <file-name> --dir=<dir-name> --url=<url-name>
```

## Options

### --imc

will view a list of exist components under /App/components, \
select all components you need to import

```js
rigel add component <component-name> --imc
```
