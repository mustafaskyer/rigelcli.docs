# Introduction
> RIGEL is a simple CLI, which should help you handle more of work in\
less time,\
and less effort

-- -


*note: make sure you have installed nodejs & git & reactNative successfully\
note: windows users, don't run from gitbash terminal*

# installaion


<!-- tabs:start -->


#### ** npm **

```
npm i -g rigel-cli
```


<!-- tabs:end -->


# commands

##### init
> rigel init app

-- -
##### Add
> add new files

<!-- tabs:start -->

#### ** screen **


```
rigel add HomeScreen
```
this will propmpt new list to select what type of file you want to add,\
select screen,\
this will create new directory under `App/Screens`,\
the created directory will contain `index.js` & `styles.js`

#### ** component **

```
rigel add InputComponent
```
This will Prompt new list to choose btween them, selec Component\
And it should create new component under `App/Components` with the `InputComponent`
#### ** reducer **


```
rigel add UserReducer
```
As Usual, A prompt list will appear, select Reducer\
this will create new reducer format under `redux/reducer`\
also by default will import the created reducer inside `redux/reducer/index`\
& will add it to exported `combineReducers` Autmoatically

#### ** action **

```
rigel add LoginAction
```
Select `Reducer Action` from the prompt list,\
this will create new reducer action under `redux/action`\
also will export the created action from `redux/actions/index`
so, you can import directly from `redux-action`


#### ** types **

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


#### ** saga **

```
rigel add user
```
Select Redux Saga from the Prompt List\
this will create new saga format under `redux/sagas`\
also will import the `watchFunction` into `redux/sagas/index`\
and will add the imported method into `all` saga method Automatically

<!-- tabs:end -->


##### Options
> accept beside commands

<!-- tabs:start -->


#### ** reduxscreen **

```
rigel add Main --reduxscreen
```
passing this option will do the following
- create types with name `main.js` inside `App/redux/types` dir & will export file from `App/redux/types/index`\
so easily can import types from `'redux-types'` alias

- create action file with name `main.js` inside `App/redux/actions` dir & will export created file from `App/redux/actions/index`\
so easily can import action from `'redux-actions'`

- create reducer file with name `mainReducer.js` inside `App/redux/reducer` dir & will import the created file inside `App/redux/reducer/index`\
imported file will add to the exported `combineReducers` func

- created saga file with name `main.js` inside `App/redux/saga` dir &\
will import the created `watchMain` func inside `App/redux/saga/index`\
also will add the imported func to `sagaroot` func

- create new dir inside `App/screens` with name `Main`\
Main Dir should contains two files\
`index.js`\
`styles.js`


*note: that created types are imported inside created action, reducer, saga*

#### ** imc **

```
rigel add Main --imc
```

- it will prompt new list of existing components under `App/components`\
select all components you need in your new screen

- all selected components will import into new screen

*note* `works only with screen type`



#### ** ima **

```
rigel add Main --imc
```

- it will prompt new list of existing actions under `App/redux/actions`\
select all actions you need in your new screen

- all selected actions will import into new screen & will added as a second parameters to `connetc` hoc

*note* `works only with screen type`


#### ** export **
```
rigel add Main --export
```
it will prompt new list to select the path you'd like to export the new screen\
this option helps you to export the new screen to specific path\
*note* `works only with screens type`


<!-- tabs:end -->