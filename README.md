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



