#ES6 CLASSES

##EXAMPLE 1 WITHOUT METHODS

```javascript

// named

var Polygon = class Polygon {
 constructor(height, width) {
   this.height = height;
   this.width = width;
 }
};
VAR hex = new Polygon(100,100)

```


##EXAMPLE  1 WITH METHODS

```javascript

class Car {
   constructor(name) {
       // - this is the newly created object
       // - anything assigned here will be assigned
       //   to the object directly
       this.kind = 'Car';
       this.name = name;
   }
// - class methods are assigned to the prototype of 
   //   the newly created object
   // - this prototype object will be shared by all instances
   printName() { 
       console.log('this.name');
   }
}

```



##ES5 EXAMPLE
```javascript
let car = new Vehicle('Tesla', 'car');
console.log(car.getName()); // Tesla
console.log(car.getType()); // car
//es5
function Vehicle (name, type) {
  this.name = name;
  this.type = type;
};
 
Vehicle.prototype.getName = function getName () {
  return this.name;
};
 
Vehicle.prototype.getType = function getType () {
  return this.type;
};
var car = new Vehicle('Tesla', 'car');
console.log(car.getName()); // Tesla
console.log(car.getType()); // car
```

##ANOTHER ES6 EXAMPLE (using SET and GET Methods)
Getter gets the VALUE of a specific PROPERTY (getting the name of the car)
Setter is a method that SETS the VALUE of a specific PROPERTY

```javascript
class Car {
 
  constructor (name) {
    this._name = name;
  } 
 
  set name (name) {
    this._name = name;
  }
 
  get name () {
    return this._name;
  }
 
}
let car = new Car('Tesla');
console.log(car.name); // Tesla
car.name = 'BMW';
console.log(car.name); // BMW
//es6
class Vehicle {
 
  constructor (name, type) {
    this.name = name;
    this.type = type;
  }
 
  getName () {
    return this.name;
  }
 
  getType () {
    return this.type;
  }
 
}


##Example: Getting and Setting 

```javascript
class GetThings
constructors(size) {
this.length = size;
}
get Length() {
   return this.length;
}
set Length (value) {
this. length = value ;
console.log(“the value has been set”);
}}

```






