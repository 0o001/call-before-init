# call-before-init
 
```js
class Before {
    [(function hello() {
        console.log('Before Initialization, I am first');
    })()]

    static {
        console.log('I am second');
    }
    
    constructor() {
       console.log('I am third but if i call');
    }
}  

/*output: Before Initialization, I am first
          I am second
*/
```