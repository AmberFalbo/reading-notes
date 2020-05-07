# Class 07 Notes (5-4-20)

Feedback Takeaways
- things on the lab are not covered in class for a reason, compares to what having a job wil be most like.
- Saturday Partner Power Hour is an option!!
- PAIR PROGRAMMING WHEN AWESOME!

DOM - Document Object Model

Code Review

Questsions - Stretch Goal #6


Old ways
```
var dinoScript = 'The numbers ' + dynamicArray[0] + ',' + dynamicArray[1] + ',' + dynamicArray[2] + ',' + dynamicArray[3]+ ',' + dynamicArray[4] + ' have a product of ' + dinoMoreOranges[0] + '.';
  console.log(dinoScript);
  return [dinoMoreOranges[0], dinoScript];

```

Template Literal
tick at the beginning and tick at the end, sees the white spaces!
Using from now on!

```
var outputString = `The numbers ${dynamicArray[0]}, ${dynamicArray[1]}, ${dynmaicArray[2]}, ${dynamicArray[3]}, ${dynamicArray[4]} have a product of $ {total}.`
return [total, outputString];
```

Refactored 
```
var outputString = `The numbers ${dynamicArray} have a product of $ {total}.`
return [total, outputString];
```

## Images

Legality of Image Use:
*unsplash.com (all free photos!!)

JPGS - bigger files - photos
PNG - bigger files - photos - transparent background(great for logos)
GIF - smaller file - logos, limited colors, animated

Size for how big you want your image to be!
Resize - Then Save

Dangers with an absolute path!

# Objects

## KEY Value pairs

```
school: 'Code Fellows'

student: 'Spencer'

teacher: 'Lena'

isCloudy: true

students: ['Courtney', 'Edgar', 'Martya']

```

// Object Literal
  // collection of key value pairs

```  
  var ilya = {
    name: 'Iyya',
    eyeColor: 'blue',
    hair: ['pink', 'blue', 'red', 'brown']
    isLoud: true,
    age: 11,
    father: {
      name: 'Adam',
      eyeColor: 'blue',
      hair: 'light brown',
      age: 40
    }
  };


var adam = {
    name: 'Adam',
    eyeColor: 'blue',
    hair: 'light brown',
    isLoud: false,
    age: 40
  };


```


## a function inside of an object is a method!



//accessing properties on an object
//1. dot notation
console.log(ilya.name)


```

var ilya = {
  name: 'Ilya',
  eyeColor: 'blue',
  hair: ['pink', 'blue', 'red', 'brown'],
  isLoud: true,
  age: 11,
  father: {
    name: 'Adam',
    eyeColor: 'blue',
    hair: 'light brown',
    age: 40
  },
  dancing: function(){
    console.log('Ilya is dancing');
  }
};


var adam = {
  name: 'Adam',
  eyeColor: 'blue',
  hair: 'light brown',
  isLoud: false,
  age: 40
};

//accessing properties on an object
//1. dot notation
console.log(ilya.hair[1])
console.log(ilya.isLoud)
console.log(ilya.father.eyeColor)

```

//2. bracket notation
console.log(ilya['name'])


bracket notation is good when you don’t know the property name!
@treebob (weird character then use bracket notation)

always invoke the method like you would a function

ilya.dancing()


making template litera;
 you must use ‘this’ when dealing with an object

```
  dancing: function(){
    console.log(`${this.name} is dancing`);
  }

```

the Contextual “this”


can access any object to be “dancing

```
var ilya = {
  name: 'Ilya',
  eyeColor: 'blue',
  hair: ['pink', 'blue', 'red', 'brown'],
  isLoud: true,
  age: 11,
  father: {
    name: 'Adam',
    eyeColor: 'blue',
    hair: 'light brown',
    age: 40,
  },
  dancing: function(){
    console.log(`${this.father.name} is dancing`);
  }
};
```

add to it!!

```
 },
  dancing: function(){
    console.log(`${this.name} and ${this.father.name} are dancing`);
  }
};
```

Ilya and Adam are dancing


Work in class!!!

```
var lucipurr = {
  name: 'Lucipurr',
  eyeColor: 'Jade',
  hair: ['Black', 'Tan', 'Golden'],
  isLoud: true,
  age: 4,
  temperment: 'Monster',
  sister: {
    name: 'Ethel',
    eyeColor: 'Green',
    hair: ['White', 'Gray', 'Tan'],
    age: 4,
    temperment: 'Sweetheart'
  },
  playing: function(){
    console.log(`${this.name} is playing with ${this.sister.name}`);
  }

};

lucipurr.playing()


console.log(lucipurr['eyeColor'])
console.log(lucipurr['temperment'])
console.log(lucipurr.sister['temperment'])
``

results

Lucipurr is playing with Ethel
Jade
Monster
Sweetheart


Adding properties to an object!!!

// to add a property:
ilya.sings = true;
console.log(ilya);


LOOPING THROUGH

```
var myPets=[
  {
    name: 'cookie',
    age: 9
  },
  {
    name: 'tangerine',
    age: 6
  },
  {
    name: 'malaki',
    age: 4
  }
]

var petNames = [];

// loop through myPets. Find just the name of my pets and push it into my petNames array

for(var i = 0; i<myPets.length; i++){
  console.log(myPets[i].name);
}
```



PUSHING and showing as an array

for(var i = 0; i<myPets.length; i++){
  petNames.push(myPets[i].name);
}


var petNames = [];

// loop through myPets. Find just the name of my pets and push it into my petNames array

for(var i = 0; i<myPets.length; i++){
  petNames.push(myPets[i].name);
}


DOT NOTATION IS LOOKING FOR A OBJECT

# DOM

loooking at 
document. —

GREAT Practice to write notes!

// Goal: add details about the pets to the DOM via the js file

// make an object literal for each animal with details
// make a render method for each animal
  // selcect a DOM parent element
  // creat a DOM li element
  // give that DOM element content
  // append it to the parent element



Salmon Cookies

object literals for each store
	min customer per hour
	max customer per hour
	avg cookie per customer
	array that holds and average number of customers for every hour the store is open 	based off of the min and max using Math.random
	array that hold the average number of cookies sold every hour at that store - multiply 	the random customers by the average cookie sale


tricks:
struggle and work tonight (will code review tomorrow to make sense)
*monday and tuesdays are always the hardest of 201*
HTML (ul wth id) & JavaScript

New Repo!! Start commiting to a branch vs. Master!!

paths for branchs
new feature/object literal/render method Math.random = new branch
