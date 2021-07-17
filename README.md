
## Syntax
```js
const async = async() =>{
  const value = await func(()=>{
      // asynchronous processing
      }).then (() => {
      // asynchronous processing success
      return 'success';
      }).catch(() => {
      // asynchronous processing fail
      return 'fail' ;
  })
}
```

## Whay useing async/await?

```js
const asyncFunc = () =>{
 const res = await fetch(''); //res is true or false 
 
 res === true ? console.log('asynchronous processing success'): 
                console.log('asynchronous processing fail')
 
};
const text="async";
const result = asyncFunc();
console.log(`${text}${result}`);
```
### Result
1. console.log(`${const}${res}`); = async,undefiend
2. console.log('asynchronous processing success'); 
