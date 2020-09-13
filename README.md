# Rap Esteva's Snippets
My custom made snippets in VS Code

## Javascript

### **class**
Creates a class Boilerplate

Passing in **classname**, **constructor method**, sample **construct parameter**, and a sample **method**.
```Javascript
class AppController{
 construct(id){
  this.id = id;
 }

 //Methods
 add(){
  //Code here
 }
}
```

### **funcprop**
Creates a function property that should be used only inside the object.
Typed in should be the **name** of the function, **parameters** and the actual code.

```Javascript
add:function(param){
 //Code here
}
```

### **insertadjacent**
Creates a starter insertAdjacentElement method.

Typed in should be the **parent element**, **child element** and the **location** to where we place the child element.

Reference:
 * **'beforebegin'** -  Before the targetElement itself.
 * **'afterbegin'** -  Just inside the targetElement, before its first child.
 * **'beforeend'** -  Just inside the targetElement, after its last child.
 * **'afterend'** -  After the targetElement itself.


```Javascript
ul.insertAdjacentElement('beforeend', li);

document.querySelector('.parent').insertAdjacentElement('beforeend', li);
```

### **createElem**
Creates a boilerplate in creating HTML Elements

Typed in should be the **element** to be created which is the `<li></li>` tags, **class** and **id**, **parent** to place the li which is `<ul>`,
then the Inner HTML thats inside the `li` tags.

```Javascript
//Create li element
   const li = document.createElement('li');
   //Add class
   li.className = 'li-class';
   // Add ID
   li.id = `liElem`;
   //Add HTML
   li.innerHTML = `
     <p> Sample Info </p>
   `;

   //Insert item
   //You can edit this
  document.querySelector('ul').insertAdjacentElement('beforeend', li);
   
```

### **iife**
Creates an iife function, that auto runs the function and puts it inside a const variable.

Typed in should be the **name** of the function, **parameters**, the **arguments** and the actual code.

```Javascript
const autoInitiate = (function(params){
  //Code here
})(params); /* Pass the arguments here */
```

### **iiferet**
Creates an iife function, that auto runs the function and sets up the 
private and public methods already.

Public methods are the ones inside the ``return`` method.

Typed in should be the **name** of the function, **parameters**, the **arguments** and the actual code.

```Javascript
const autoRun = (function(params){
 /* Private Methods */
  add:function(){
   //Code here
  };


  /* Public Methods */
  return{
   init:function(){
    
   }
  }
  
})(params); 
```

### **listen**
creates a starter event listener, with a callback.

Typed in is the **element**, **event**, **params** and actual code.
```Javascript
elem.addEventListener('click', (e)=> {
  //Code here
});
```

### **listenfunc**
creates a starter event listener, but instead it calls back a defined ready function.

Typed in is the **element**, **event**, **function name**.
```Javascript
elem.addEventListener('click', add(params));
```

### **select**
creates a query selector.

Typed in is the html tag, class or id.
```Javascript
document.querySelector('.btn-primary');
```

### **select**
creates a query selector all.
It should be an array of html elements.

Typed in is the html tag, class or id.
```Javascript
document.querySelectorAll('.list');
```

### **prevent**
Creates a prevent default method

Typed in is the element with the link.
Usually used for buttons and anchor tags.

```Javascript
e.preventDefault();
```


### **fetch**
Creates a fetch boilerplate with then and catch statements. 

```Javascript
fetch('url')
 .then(response => response.json())
 .then(json => console.log(json))
 .catch(err => console.log(err));
```

### **fetch2**
Creates a 2nd fetch boilerplate with then and catch statements. 

```Javascript
fetch(url)
   .then(response => {
     return response.json();
   })
   .then(json => {
     console.log(json);
   })
   .catch(err => {
     console.log(err);
   });
```

### **funcpromise**
Converts a function to a promise.

```Javascript
function name(argument){
  return new Promise((resolve, reject)) => {

  if(!argument){
    reject(new Error('return this when theres an error'));
  }else{
    setTimeout(resolve, argument);
  }
  
  }
}
```

### **funcasync**
Converts a function to a promise but in async form.

```Javascript
async function name(argument){
   let api = 'url';
   let response = await fetch(api);
   let json = await response.json();

   return{
     result:json
   }
 }
```

### **metasync**
Converts a method to a promise but in async form.
This needs to be used inside a Class

```Javascript
async name(argument){
   let api = 'url';
   let response = await fetch(api);
   let json = await response.json();

   return{
     result:json
   }
 }
```

### **fetchfunc**
Creates a fetch boilerplate to attach to a promisified function

```Javascript
funcName()
  .then(data => {
    console.log(data.result);
  })
  .catch(err => console.log(err));
```

### **randomnum**
A random number from 0 up to any number you like.

9 for example.

```Javascript
const randomNum = Math.floor(Math.random() * Math.floor(9));
```

### **randomarr**
Creates a random num based on the length of the array.

```Javascript
const length = array.length;
const randomNum = Math.floor(length * Math.random()); 
```


