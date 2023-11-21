# JavaScript - 2 - Looping
```
let myArray = [1, 2, 3, 4, 5];

for (let i = 0; i < myArray.length; i++) {
    console.log(myArray[i]);
}
myArray.forEach(item => {
    console.log(item);
});

//Looping Through an Object:

let myObject = {
    key1: 'value1',
    key2: 'value2',
    key3: 'value3'
};

for (let key in myObject) {
    console.log(key + ': ' + myObject[key]);
}
Object.keys(myObject).forEach(key => {
    console.log(key + ': ' + myObject[key]);
});


//Looping Through an Array of Objects (Direct Access):

let arrayOfObjects = [
    { name: 'John', age: 25 },
    { name: 'Jane', age: 30 },
    { name: 'Bob', age: 22 }
];

for (let i = 0; i < arrayOfObjects.length; i++) {
    console.log(arrayOfObjects[i].name + ': ' + arrayOfObjects[i].age);
}
arrayOfObjects.forEach(obj => {
    console.log(obj.name + ': ' + obj.age);
});

//Looping Through an Array of Objects (Dynamic Key Names):

let arrayOfObjectsDynamic = [
    { prop1: 'value1', prop2: 'value2' },
    { prop1: 'value3', prop2: 'value4' },
    { prop1: 'value5', prop2: 'value6' }
];

for (let i = 0; i < arrayOfObjectsDynamic.length; i++) {
    for (let key in arrayOfObjectsDynamic[i]) {
        console.log(key + ': ' + arrayOfObjectsDynamic[i][key]);
    }
}
// Or using forEach and Object.keys
arrayOfObjectsDynamic.forEach(obj => {
    Object.keys(obj).forEach(key => {
        console.log(key + ': ' + obj[key]);
    });
});
```
# output
![image](https://github.com/21002624/-Looping/assets/113762183/ec8fab6e-2b09-4a3c-86f8-34258ebf038f)
