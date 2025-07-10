const product = {
    name : "parker ball pen",
    rating : 4,
    offer : 5,
    price : 270,

};
const profile = {
 name : "Shradda khapra",
 isFollow : "true",
 
 followers : 243,
 following : 4,
 

};

// arithmetic operators
let a=10;
let b=5;

console.log("a=",a ,"& b=",b);
console.log("a+b=",a+b);
console.log("a-b=",a-b);
console.log("a/b=",a/b);
console.log("a * b=",a*b);
console.log("a % b=",a%b);
console.log("a ** b=",a**b);

//assignment operators
let a=10;
let b=5;

a+=5; //a=a+5
console.log("a=",a);
b-=2; //b=b+2
console.log("b=",b);

// comparison operators

let a=10;
let b=5;

console.log("a==b",a==b);//false
console.log("a!=b",a!=b);//true
console.log("a===b",a===b);//false
console.log("a!==b",a!==b);//true
console.log("a<b",a<b);//false
console.log("a<=b",a<=b);//false
console.log("a>=b",a>=b);//true
console.log("a>=b",a>=b);//true

//logical operators

let a=10;
let b=5;

console.log("cond1 && cond2 =", a>b && a==10); //true

console.log("cond1 || cond2 =", a<b || a==10); //true

console.log("10>5 =", !(a>b)); //false 

// if statement

age = 15;

if(age>=18)
{console.log("you can vote")}

if(age<18)
{ console.log("you cannot vote")}

let num = prompt("Enter a number =");

if(num%5===0)
{
    console.log(num,"number is divisible by 5");
}
else{
    console.log(num,"number is not divisible by 5");
}


// calculate sum of 1 to 10
let sum=0;
for(let i=1; i<=10; i++)
{
    sum=sum + i;
    
}
console.log("sum=",sum);

for count numbers from 1 to 10

for(let i=0; i<=10; i++)
{
    console.log("i =",i);
}

while loop

let i=1;
while(i<=10)
{
    console.log("i=",i);
    i++;
}

do while loop

let i=1;
do
{
    console.log("i=",i);
    i++;
}
while(i<=10)

// for-in loop - which is mainly used for 1- Strings and arrays

let string = "Jagdeep";
let size = 0;

for(let val of string){

    console.log("val", val)
    size++;
}
console.log("Size of string =", size);

// for-in loop - which is mainly used for 1- objects and arrays

let student={
    name : "jagdeep singh",
    age : 21,
    cgpa : 89.6,
    isPass : "true"
};

for(let key in student){

  console.log("key = ", key,  "value",student[key]);
}

// practice q1 --

for(i=1; i<=100; i++){

    if(i%2===0)
    {console.log("i = ", i)};
}

// practice q2 --

let gameNum = 30;
let userNum = prompt("Guess the number :");

while(userNum != gameNum){
    userNum = prompt(" you guessed the wrong number, guess again :");
}
console.log("congratulations, you guessed right number");

let str = "Jagdeep Singh";

console.log(str.length);
console.log(str);

let obj={
    item : "pen" ,
    price : 10,
};
let output = `The price of the ${obj.item} is ${obj.price} rupees`;
console.log(output);

let str="Jagdeep singh";
let newStr = str.toUpperCase();

console.log(str);
console.log(newStr);

let str="MANMOHAN SINGH";
let newStr = str.toLowerCase();

console.log(str);
console.log(newStr);

// practice question 3
let fullName = prompt("Enter your fullName without spaces :");

let username = "@" + fullName + fullName.length;
console.log(username);

// arrays

let marks=[99,92,95,78,79];

console.log(marks);

//accessing arrays with the help of loops

let heroes = ["superman", "batman" , "hulk", "spiderman", "ironman"];

for(let idx=0; idx<heroes.length; idx++){
    console.log(heroes[idx]);
}


// for-of

for(let hero of heroes){
    console.log(hero)
}
// practice question 4

let marks=[90,89,78,67,76];
sum=0;
for(let val of marks){
    sum+=val;
}
let avg = sum/marks.length;
console.log( `The average marks of the class is = ${avg} `);

// practice question 5

let arr=[250,645,300,900,50];
let i=0;
for(let val of arr){
    console.log(`value at index ${i} = ${val}`)
   let offer = val/10;
   arr[i] = arr[i]-offer;
   console.log(`value after 10% offer is : ${arr[i]}`);
   i++;
}


array methods

1)- PUSH methods

let veggies =["potato" , "tomato", "carrot", "raddish"];

console.log(veggies);
veggies.push("baigan");
console.log(veggies);

2)- pop methods

let veggies =["potato" , "tomato", "carrot", "raddish"];

console.log(veggies);

let deletedItem = veggies.pop();
console.log(veggies);
console.log("deleted Item :", deletedItem);

3)- tostring() methods

let marks=[97,28,72,45,66];

console.log(marks.toString());

4)- concat - join multiple array & give result

let marvelHeroes = ["Iron man", "Hult","captain america"];
let dcHeroes=["Batman", "Joker", "superman"];

let heroes = marvelHeroes.concat(dcHeroes);
console.log(heroes);

5)- slice() method - returns a piece of array.

let marvelHeroes = ["Iron man", "Hulk","captain america", "Ant man"];
console.log(marvelHeroes);
console.log(marvelHeroes.slice(1,3));

6)- splice()- change original array (add, remove, replace).

let arr = [1,2,3,4,5,6,7];

//  let val=arr.splice(2,2,101,102);

// add new number
arr.splice(2,0,101);

7)- shift-

let companies = ["bloomberg", "microsoft", "uber", "google", "Ibm","netflix"];
console.log(companies);

let val=companies.shift();

console.log("deleted item", val);

let companies = ["bloomberg", "microsoft", "uber", "google", "Ibm","netflix"];
console.log(companies);


let val=companies.splice(2,1,"ola");
console.log(val);


let companies = ["bloomberg", "microsoft", "uber", "google", "Ibm","netflix"];
console.log(companies);

companies.push("amazon");
console.log(companies);

// Functions

function myFun (){
    console.log("hello");
     console.log("Bye");
}

myFun();

// parameter in function

function myFun (msg){
    // paramter--> input
    console.log(msg);
     
}

// argument
myFun("how are you");

function sum (x,y){
  sum=x+y;
  return sum; 
  
}
let val = sum (5,5);
console.log(val);

//  arrow Functions

let multi = (a,b) => {
    console.log(a*b);
}


practice question

function countVowels(str) {

     let count=0;
    for(let char of str){
        if(char === "a" || char === "e"||char === "i"||char === "o"||char === "u"){
            count ++;
        }
        }
        console.log(count);
    }

    // using arrow function

     let countVow = (str) => {
          let count=0;
    for(let char of str){
        if(char === "a" || char === "e"||char === "i"||char === "o"||char === "u"){
            count ++;
        }
        }
        console.log(count);
    }

    // forEach function

    let arr = ["Rohtak", "Rewari", "Hisar"];

arr.forEach((val,idx,arr)=>{
    console.log(val.toUpperCase(),idx,arr);
});

let arr = [1,2,3,4,5];
arr.forEach((arr)=>{
    console.log(arr*arr);
});

// map function is used in creating a new array from a array it is different from forEach method

let arr = [1,2,3,4,5];

let newArr=arr.map((val)=>{
   
    return(val*2);
});
 console.log(newArr);

 // filter function 

 let arr = [1,2,3,4,5];

let newArr=arr.filter((val)=>{
   
    return(val%2==0);
});
 console.log(newArr);

 // reduce method

 let arr = [1,2,3,4,5];

let newArr=arr.reduce((res,curr)=>{
    return res+curr;
});
console.log(newArr);

//to save greater number in the output

let arr = [1,2,3,20,5];

let output=arr.reduce((pre,curr)=>{
    return pre>curr?pre:curr;
});
console.log(output);


let marks = [80,99,90,78,95,67];

let highest=marks.filter((val)=>{
    return(val>=90);
})
console.log(highest);

// sum of numbers and factorial of numbers
let n = prompt("Enter a number :");

let arr = [];
for ( let i=1; i<=n; i++){
    arr[i-1]=i;
}
console.log(arr);
let val= arr.reduce((prev,curr)=>{
    return prev+curr;
}
)
console.log("sum :", val);


let factorial= arr.reduce((prev,curr)=>{
    return prev*curr;
}
)
console.log("factorial :", factorial);


let divs = document.querySelectorAll(".box");
let idx=1;
for(let div of divs){
    div.innerText = `new value ${idx}`;
    idx++;
}

let newBtn = document.createElement("button");
newBtn. innerText = "click me!";

newBtn.style.color = "white";
newBtn.style. backgroundColor = "red";

document. querySelector ("body"). prepend (newBtn);

let btn1 = document.querySelector("#btn1");
btn1.onclick = () => {
    console.log("button is clicked");
    let a=25;
    a++
    console.log(a);
}
let div=document.querySelector("div");
div.onmouseover = () => {
 console.log("you are on div");
}

// event listner 

let btn1 = document.querySelector("#btn1");

btn1.addEventListener ( "click", (evt) => {
console. log ("buttoni was clicked - handler1");

});

btn1.addEventListener ( "click", (evt) => {
console. log ("buttoni was clicked - handler2");
});

const handler3 = (evt) => {
console. log ("buttoni was clicked - handler3");
};

btn1.addEventListener ( "click", handler3);

btn1.addEventListener ( "click", (evt) => {
console. log ("buttoni was clicked - handler4");
});

btn1.removeEventListener ( "click", handler3 );

// toggle of color change

let modeBtn = document.querySelector("#mode");
let body = document.querySelector("body");
let currMode = "light";

modeBtn.addEventListener("click", () => {
    if(currMode === "light"){
        currMode = "dark";
        body.classList.add("dark");
        body.classList.remove("light");
    }
    else {
        currMode = "light";
        body.classList.add("light");
        body.classList.remove("dark");
    }
    console.log(currMode);

})

// css for toggle

.dark {
    background-color: black;
    color: white;
}
.light {
    background-color: white;
    color: black;
}