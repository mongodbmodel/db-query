# DB Query

 Standalone base module extending the NodeJs Transform API with few other functionalities added

### Installation

```bash
$ yarn add @eweah/db-query 

```
 or 

```bash

$ npm i @eweah/db-query

```

### Simple Usage Example

```bash
 const Base = require('@eweah/db-query');
 const base = new Base();
 base.apiGet();
 base.on('apiGet', data => console.log(data));
 base.on('apiGet-error', error => console.error(error));
 
```
or 
```bash
 class MyWonderfulClass extends require('@eweah/db-query') {

    constructor(...arrayOfObjects) {

    super({ objectMode: true, encoding: "utf-8", autoDestroy: true });

    arrayOfObjects.forEach(option => {
        if(Object.keys(option).length > 0){
            Object.keys(option).forEach((key) => { if(!this[key]) this[key] = option[key];})
        }
    });

    this.autobind(MyWonderfulClass);
    this.autoinvoker(MyWonderfulClass);
    this.setMaxListeners(Infinity);
  }
 };
 
```


