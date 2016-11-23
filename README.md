ES6 CLASSES

# EXAMPLE 1 WITHOUT METHODS

// named
var Polygon = class Polygon {
 constructor(height, width) {
   this.height = height;
   this.width = width;
 }
};
VAR hex = new Polygon(100,100)


# EXAMPLE  1 WITH METHODS
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
var mazda = new Car('Mazda');








