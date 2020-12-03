Class 07
[Back to 201 Index](./../201-index.md)<br>

Tables

<table>	
	<tr>


  Constructor functions

```

// var sarah = {
//   name: 'Sarah',
//   hair: 'brown',
//   eyes: 'green',
//   student: true,
//   shoesSize: 8.5,
//   doingLab: function(){
//     console.log(`${this.name} is dong lab`)
//   }
// }

// var andrew = {
//   name: 'Andrew',
//   hair: 'brown',
//   eyes: 'blue',
//   student: true,
//   shoeSize: 10.5,
//   doingLab: function(){
//     console.log(`${this.name} is dong lab`)
//   }
// }

function Student(name, hair, eye, shoeSize){
  this.name = name;
  this.hairColor = hair;
  this.eyeColor = eye;
  this. shoeSize = shoeSize;
}

var sarah = new Student('Sarah', 'brown', 'green', 8.5); 
var andrew = new Student('Andrew', 'brown', 'blue', 10.5);

console.log(sarah, andrew)


adding function as method

function Student(name, hair, eye, shoeSize){
  this.name = name;
  this.hairColor = hair;
  this.eyeColor = eye;
  this. shoeSize = shoeSize;
  this.doingLab = function(){
    console.log(`${this.name} is dong lab`);
  };
}

var sarah = new Student('Sarah', 'brown', 'green', 8.5); 
var andrew = new Student('Andrew', 'brown', 'blue', 10.5);

sarah.doingLab();



pulling methods(previous functions) and pulling them and turning into this!!
(only works on constructor functions)

Student.prototype.doingLab = function(){
    console.log(`${this.name} is dong lab`);
  };

```

[Back to 201 Index](./../201-index.md)<br>