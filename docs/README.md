# Introduction
> RIGEL is a simple CLI, which should help you handle more of work in\
less time,\
and less effort

-- -

# installaion
using npm
```
npm i -g rigel-cli
```
using yarn
```
yarn add global rigel-cli
```
# commands
### initialize new app
> rigel init app

-- -
### Add
### Screen

```
rigel add HomeScreen
```
this will propmpt new list to select what type of file you want to add,\
select screen,\
this will create new directory under `App/Screens`,\
the created directory will contain `index.js` & `styles.js`

-- -

### Component

```
rigel add InputComponent
```
This will Prompt new list to choose btween them, selec Component\
And it should create new component under `App/Components` with the `InputComponent`

-- -

### Reducer
```
rigel add UserReducer
```
As Usual, A prompt list will appear, select Reducer\
this will create new reducer format under `redux/reducer`\
also by default will import the created reducer inside `redux/reducer/index`\
& will add it to exported `combineReducers` Autmoatically

-- -

### Reducer Action
```
rigel add LoginAction
```
Select `Reducer Action` from the prompt list,\
this will create new reducer action under `redux/action`\
also will export the created action from `redux/actions/index`
so, you can import directly from `redux-action`

-- -

### Reducer Types
```
rigel add user
```
Select Reducer Types from The Prompt List,\
this will create new type format under `redux/types`
also will export the types from `redux/types/index`
types format
    - USER_CASE
    - USER_CASE_SUCCESS
    - USER_CASE_FAILED\

so, you will be able to import types directly from `redux-types`

-- -

### Reducer Sagas
```
rigel add user
```
Select Redux Saga from the Prompt List\
this will create new saga format under `redux/sagas`\
also will import the `watchFunction` into `redux/sagas/index`\
and will add the imported method into `all` saga method Automatically

-- -

### Options

#### --imc
it will prompt new list of existing components\
after select all components you need in your new screen,
you will go to the new propmt list to select file type, which should be screen

*this option helps you to import components into new screens*\
*note* `works only with screen type`
-- -

### --ima
it will prompt new list of existing actions\
after select all actions you need,\
you will move to next propt to select file type, which should be screen

*this option helps you to import actions into new screen*\
*and will add the imported action to the `connect` redux hoc*\
*note* `works only with screens type`
-- -

### --export
it will prompt new list to select the path you'd like to export the new screen\
this option helps you to export the new screen to specific path\
*note* `works only with screens type`
