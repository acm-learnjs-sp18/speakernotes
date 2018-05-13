Kevin's Intro- these are spring events and whatnot

Welcome to the first workshop of Learn.js! Today we'll be going over an introduction to JavaScript syntax and a few things you should know especially if you're coming from a different programming language.

You can find the starter code at this GitHub link and you can just download the ZIP by clicking that big bright green button they have. If you're not familiar with GitHub, do not worry! There is a direct download link on the Facebook Event page under "Discussion." And throughout this session, I'm going to be reminding you that we have mentors all around the room assigned to every area so if you need help at any point for anything, just ask them.

Also, on the GitHub you'll find the README which goes over a bit more detail than we time to cover today, so if you want to understand everything maybe a little bit better, you can take a look at that as well.

[Schedule]

[Course Outline]

ES6+ is going to cover some of the newer and very cool features introduced into JavaScript since 2015 that make JavaScript way more powerful than anything you'll see today so make to come out to that! It'll also help you a lot in our later workshops, including...

Templating! Which allows you to make your websites more dynamic and interactive in a much simpler way.

To see JavaScript in action on the backend, come to our workshop on Node.js and Express, which are big big names for development.

D3 which is for some really cool data visualization projects. If you're into stats or data analysis or even just like pretty graphs, then you'll love D3

And React, a tool made and used by Facebook to allow you to use HTML in your JavaScript, which is really really useful and it's really big right now.

[Membership Attendance Code]

And with that out of the way...

It is time for our code-a-long and your introduction to JavaScript

[Open incognito tab]

```javascript
//explain a variable is just a way to store a value for later
//explain var keyword
//explain assignment
//semicolons are not stricly necessary in js but we use them to avoid errors/bugs
var ourFirstVariable = 5;
ourFirstVariable;
//5
//explain you can reassign the kinds of values in javascript
//although for similar reasons to avoid bugs this is not recommended
ourFirstVariable = 10;
//10
//strings and you can change the types of values you store
//explain strings (text = string of letters or characters)
ourFirstVariable = "JavaScript Rules!";
//"JavaScript Rules!"
var ourSecondVariable = 13;
//if you want to read more about this ('this' being checking for equality)
//it's on the README
ourFirstVariable === ourSecondVariable;
//false
//evaluating equality is really important for things like if statements
//which allow you to control what code actually gets run
if (ourSecondVariable === 13) {
    console.log("ourSecondVariable is 13!");
} else {
    console.log("Uh-oh!");
}
//ourSecondVariable is 13!
//introduce a new kind of variable which allows you to store multiple different kinds of data at once
var anArray = [4, "Learn.js", true];
//if you're coming from C++ or Swift or anything like that you'll notice that we actually have different kinds of data in our array, we have a number a string and the value true
anArray;
//(3) [4, "Learn.js", true];
anArray[0];
//4
anArray[1];
//"Learn.js"
//ok i'm gonna throw a few different things at you guys right now so if u have any questions please ask a mentor!
//code first
for (var counter = 0; counter < 3; counter++) {
    console.log(anArray[counter]);
}
//explain after
//starting this variable at 0, we're going to go so long as it is less than 3 and we're going to move through the loop by increasing counter by 1
//and every time we move through this loop we're going to print out the value in the array that corresponds to the counter
function myFunction() {
    console.log("I am a function!");
}
myFunction();
//"I am a function!"
//don't forget the parentheses!
function myNewFunction(name) {
    console.log(name);
}
myNewFunction("dustin");
//ok now for the last thing you'll need to build a super cool JavaScript project
var myObject = {
    name: "Dustin",
    age: 19
};
myObject.name;
//"Dustin"
myObject.age;
//19
```

I hope you were paying attention because now it's time for Kahoot!

[Demo]

```javascript
var time = document.getElementById("clock");
//think of this global document object and how do we access the properties of an object? DOTS!
var hex = document.getElementById("hex");
var body = document.getElementById("body");

function updateClock() {
    var date = new Date();
    var hours = date.getHours();
    var minutes = date.getMinutes();
    var seconds = date.getSeconds();
    var ampm = "";

    var dateFormat = ['h', 'm', 's'];

    var color = time2color(dateFormat, hours, minutes, seconds);

    if (hours >= 12) {
        ampm = "PM";
    } else {
        ampm = "AM";
    }

    if (seconds < 10) {
        seconds = "0" + seconds;
    }
    if (minutes < 10) {
        minutes = "0" + minutes;
    }

    if (hours != 12) {
        hours %= 12;
    }

    time.innerHTML = hours + ":" + minutes + ":" + seconds + " " + ampm;

    hex.innerHTML = "#" + color;

    body.style.backgroundColor = color;
};
updateClock();
setInterval(updateClock, 1000);

function time2color(dateFormat, hours, minutes, seconds) {
    var result = [];
    for (var i=0; i < dateFormat.length; i++) {
        switch(dateFormat[i]) {
            case 'h':
                result.push(dec2hex(hours / 24));
                break;
            case 'm':
                result.push(dec2hex(minutes / 60));
                break;
            case 's':
                result.push(dec2hex(seconds / 60));
                break;
        }
    };
    return result.join('');
}
```

In case of emergency

```javascript
function dec2hex(d) {
    d = parseInt(d * 255);
    var hex = Number(d).toString(16);
    padding = typeof(padding) === "undefined" || padding === null ? padding = 2 : padding;
    while (hex.length < padding) {
        hex = "0" + hex;
    }
    return hex;
}
```

