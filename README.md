# datastructures

#### basics

creating class in javascript

``` javascript
function Building(floors){

    // behind the scenes->this={} 
    this.what="building";
    this.floors=floors
    //return this;
}
var myHouse=new Building(3);//{what: "Building", floors: 3}
```

``` javascript
Building.prototype.countFloors=function(){
console.log("I have",this.floors,'floors')}
myHouse.countFloors();// I have 3 floors
// so why we use prototype 
//  because if we wont use prototype every time we call a constructor funtion,
//   it will create new instances of the countFloors function
```

