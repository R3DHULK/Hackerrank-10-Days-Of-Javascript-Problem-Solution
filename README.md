![10 Days of Javascript](10%20Days%20of%20Javascript.png)
<h1><b> 10 Days of JavaScript Solutions 👇</h1></b>
<h2><b> Day 0: Hello World: </h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

/**
*   A line of code that prints "Hello, World!" on a new line is provided in the editor. 
*   Write a second line of code that prints the contents of 'parameterVariable' on a new line.
*
*    Parameter:
*   parameterVariable - A string of text.
**/
function greeting(parameterVariable) {
    // This line prints 'Hello, World!' to the console:
    console.log('Hello, World!');
    console.log (parameterVariable);

    // Write a line of code that prints parameterVariable to stdout using console.log:
    
}
```

#

<h2><b> Day 0: Data Types: </h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

function performOperation(secondInteger, secondDecimal, secondString) {
    // Declare a variable named 'firstInteger' and initialize with integer value 4.
    const firstInteger = 4;
    
    // Declare a variable named 'firstDecimal' and initialize with floating-point value 4.0.
    const firstDecimal = 4.0;
    
    // Declare a variable named 'firstString' and initialize with the string "HackerRank".
    const firstString = 'HackerRank ';
    
    // Write code that uses console.log to print the sum of the 'firstInteger' and 'secondInteger' (converted to a Number        type) on a new line.
    console.log(firstInteger + parseInt(secondInteger));
    
    // Write code that uses console.log to print the sum of 'firstDecimal' and 'secondDecimal' (converted to a Number            type) on a new line.
    console.log(firstDecimal + parseFloat(secondDecimal));
    
    // Write code that uses console.log to print the concatenation of 'firstString' and 'secondString' on a new line. The        variable 'firstString' must be printed first.
    console.log(firstString + secondString);
}


function main() {
    const secondInteger = readLine();
    const secondDecimal = readLine();
    const secondString = readLine();
    
    performOperation(secondInteger, secondDecimal, secondString);
}

```
#

<h2><b> Day 1: Arithmetic Operators: </h2></b>

```

'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

function getArea(length, width) {
    let area;
    // Write your code here
    area = length * width;
    return area;
}


function getPerimeter(length, width) {
    let perimeter;
    // Write your code here
    perimeter=2 * (length + width);
    return perimeter;
}


function main() {
    const length = +(readLine());
    const width = +(readLine());
    
    console.log(getArea(length, width));
    console.log(getPerimeter(length, width));
}

```
#

<h2><b> Day 1: Functions: </h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}
/*
 * Create the function factorial here
 */
function factorial(n)
{
    let e=1;
    for(n;n>1;n--)
        e=e*n;
    return e;
}


function main() {
    const n = +(readLine());
    
    console.log(factorial(n));
}
```
#

<h2><b> Day 1: Let and Const: </h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

function main() {
    // Write your code here. Read input using 'readLine()' and print output using 'console.log()'.
    let s=readLine();
    // Print the area of the circle:
    console.log(Math.PI*s*s);
    // Print the perimeter of the circle:
    console.log(Math.PI*2*s);

    try {    
        // Attempt to redefine the value of constant variable PI
        PI = 0;
        // Attempt to print the value of PI
        console.log(PI);
    } catch(error) {
        console.error("You correctly declared 'PI' as a constant.");
    }
}

```
#

<h2><b> Day 2: Conditional Statements: If-Else: </h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

function getGrade(score) {
    let grade;
    // Write your code here
     if ((score > 25) && (score <= 30))
    {
        grade = 'A';
    }

    else if ((score > 20) && (score <= 25))
    {
        grade = 'B';
    }
    
    else if ((score > 15) && (score <= 20))
    {
        grade = 'C';
    }
    
    else if ((score > 10) && (score <= 15))
    {
        grade = 'D';
    }
    
    else if ((score > 5) && (score <= 10))
    {
        grade = 'E';
    }
    
    else if ((score > 0) && (score <= 5))
    {
        grade = 'F';
    }

    return grade;
}


function main() {
    const score = +(readLine());
    
    console.log(getGrade(score));
}

```


#

<h2><b> Day 2: Conditional Statements: Switch: </h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}


function getLetter(s) {
    let letter;
    // Write your code here
    //    s=[a,e,i,o,u]
    switch (s.charAt(0))
    {
        case ('a'||'e'||'i'||'o'||'u'):
        letter='A';
        break;

        case ('b'||'c'||'d'||'f'||'g'):
        letter='B';
        break;

        case ('h'||'j'||'k'||'l'||'m'):
        letter='C';
        break;

        case ('z'||'n'||'p'||'q'||'r'||'s'||'t'||'v'||'w'||'x'||'y'):
        letter='D';
        break;
    }   
    return letter;
}


function main() {
    const s = readLine();
    
    console.log(getLetter(s));
}

```
#

<h2><b> Day 2: Loops: </h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

/*
 * Complete the vowelsAndConsonants function.
 * Print your output using 'console.log()'.
 */
function vowelsAndConsonants(s) {
    var vowels=['a','e','i','o','u']
    for (var i=0; i< s.length; i++)
    {
        if (vowels.indexOf(s[i])>-1)
        {
            console.log(s[i]);
        }
    }
    for (var j=0; j<s.length; j++)
    {
        if (vowels.indexOf(s[j])<0)
        {
            console.log(s[j]);
        }
    }
}


function main() {
    const s = readLine();
    
    vowelsAndConsonants(s);
}

```
#

<h2><b>Day 3: Arrays: </h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

/**
*   Return the second largest number in the array.
*   @param {Number[]} nums - An array of numbers.
*   @return {Number} The second largest number in the array.
**/
function getSecondLargest(nums) {
    // Complete the function
    var sorted_array=nums.sort (function (a,b) {return a-b});
    var unique_sorted_array =sorted_array.filter(function(elem, index,  self)
    {
        return index==self.indexOf(elem);
    })
    return unique_sorted_array[unique_sorted_array.length - 2];
}


function main() {
    const n = +(readLine());
    const nums = readLine().split(' ').map(Number);
    
    console.log(getSecondLargest(nums));
}
```
#

<h2><b>Day 3: Try, Catch, and Finally: </h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

/*
 * Complete the reverseString function
 * Use console.log() to print to stdout.
 */
function reverseString(s) {
    try
    {
        var splitString=s.split("");
        var rverseArray=splitString.reverse();
        var joinArray=rverseArray.join("");
        console.log(joinArray);
    }
    catch (error)
    {
        console.log(error.message);
        console.log(s);
    }
}



function main() {
    const s = eval(readLine());
    
    reverseString(s);
}
```
#

<h2><b>Day 3: Throw: </h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

/*
 * Complete the isPositive function.
 * If 'a' is positive, return "YES".
 * If 'a' is 0, throw an Error with the message "Zero Error"
 * If 'a' is negative, throw an Error with the message "Negative Error"
 */
function isPositive(a) {
    if (a>0)
    {
        return "YES";
    }
    if (a==0)
    {
        throw new Error("Zero Error")
    }
    {
        if (a<0)
        {
            throw new Error("Negative Error")
        }
    }
}


function main() {
    const n = +(readLine());
    
    for (let i = 0; i < n; i++) {
        const a = +(readLine());
      
        try {
            console.log(isPositive(a));
        } catch (e) {
            console.log(e.message);
        }
    }
}
```

#

<h2><b> Day 4: Create a Rectangle Object: </h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

/*
 * Complete the Rectangle function
 */

function Rectangle(a, b) {
    this.length=a;
    this.width=b;
    this.perimeter=2*(a+b);
    this.area=a*b;
}


function main() {
    const a = +(readLine());
    const b = +(readLine());
    
    const rec = new Rectangle(a, b);
    
    console.log(rec.length);
    console.log(rec.width);
    console.log(rec.perimeter);
    console.log(rec.area);
}
```
#

<h2><b> Day 4: Count Objects: </h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

/*
 * Return a count of the total number of objects 'o' satisfying o.x == o.y.
 * 
 * Parameter(s):
 * objects: an array of objects with integer properties 'x' and 'y'
 */
function getCount(objects) {
    var count=0;
    for (var index in objects)
    {
        if (objects[index].x==objects[index].y)   
        {
            count++;
        }
    }
    return count;
}

function main() {
    const n = +(readLine());
    let objects = [];
    
    for (let i = 0; i < n; i++) {
        const [a, b] = readLine().split(' ');
        
        objects.push({x: +(a), y: +(b)});
    }
    
    console.log(getCount(objects));
}
```
#

<h2><b> Day 4: Classes: </h2></b>

```

/*
 * Implement a Polygon class with the following properties:
 * 1. A constructor that takes an array of integer side lengths.
 * 2. A 'perimeter' method that returns the sum of the Polygon's side lengths.
 */
class Polygon {
    constructor(heights) 
    {
        var polygon_perimeter = 0;
        for (var index in heights)
            {
                polygon_perimeter =polygon_perimeter+ heights[index];
            }        
        this.my_perimeter = polygon_perimeter;
    }
         perimeter() 
    {
        return this.my_perimeter;
    }
}

const rectangle = new Polygon([10, 20, 10, 20]);
const square = new Polygon([10, 10, 10, 10]);
const pentagon = new Polygon([10, 20, 30, 40, 43]);

console.log(rectangle.perimeter());
console.log(square.perimeter());
console.log(pentagon.perimeter());

```
#

<h2><b> Day 5: Inheritance: </h2></b>

```
class Rectangle {
    constructor(w, h) {
        this.w = w;
        this.h = h;
    }
}

/*
 *  Write code that adds an 'area' method to the Rectangle class' prototype
 */

/*
 * Create a Square class that inherits from Rectangle and implement its class constructor
 */

Rectangle.prototype.area=function()
{
    return (this.w*this.h)
};
/*
 * Create a Square class that inherits from Rectangle and implement its class constructor
 */
class Square extends Rectangle {
        constructor(s) {
            super(s);
            this.h = s;
            this.w = s;
        }
    };


if (JSON.stringify(Object.getOwnPropertyNames(Square.prototype)) === JSON.stringify([ 'constructor' ])) {
    const rec = new Rectangle(3, 4);
    const sqr = new Square(3);
    
    console.log(rec.area());
    console.log(sqr.area());
} else {
    console.log(-1);
    console.log(-1);
}
```
#

<h2><b> Day 5: Template Literals: </h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

/*
 * Determine the original side lengths and return an array:
 * - The first element is the length of the shorter side
 * - The second element is the length of the longer side
 * 
 * Parameter(s):
 * literals: The tagged template literal's array of strings.
 * expressions: The tagged template literal's array of expression values (i.e., [area, perimeter]).
 */
function sides(literals, ...expressions) {
    var area = expressions[0];
    var perimeter = expressions[1];
    var s1 = (perimeter + Math.sqrt(perimeter * perimeter  - (16 * area))) / 4;
    //console.log("s1: " + s1);
    var s2 = (perimeter - Math.sqrt(perimeter * perimeter  - (16 * area))) / 4;
    //console.log("s2: " + s2);
    var array = [s1, s2];
    array =  array.sort(function (a,b) {return a-b;});
    return array;

}


function main() {
    let s1 = +(readLine());
    let s2 = +(readLine());
    
    [s1, s2] = [s1, s2].sort();
    
    const [x, y] = sides`The area is: ${s1 * s2}.\nThe perimeter is: ${2 * (s1 + s2)}.`;
    
    console.log((s1 === x) ? s1 : -1);
    console.log((s2 === y) ? s2 : -1);
}
```

#

<h2><b> Day 5: Arrow Functions: </h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

/*
 * Modify and return the array so that all even elements are doubled and all odd elements are tripled.
 * 
 * Parameter(s):
 * nums: An array of numbers.
 */
function modifyArray(nums) {
    const func = nums.map(function(num)
    {
        if (num%2==0)
        {
            return 2* num;
        }
        else
        {
            return 3*num;
        }
    });
    return func;
}


function main() {
    const n = +(readLine());
    const a = readLine().split(' ').map(Number);
    
    console.log(modifyArray(a).toString().split(',').join(' '));
}
```
#

<h2><b> Day 6: Bitwise Operators: </h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

function getMaxLessThanK(n, k) {

    var mx = -1;

    for(var i=1; i<=n; i++){
        for(var j=i+1; j<=n; j++){
            var res = i & j;
            if(res > mx && res < k){
                mx = res;
            }
        }
    }
    return mx;

};


function main() {
    const q = +(readLine());
    
    for (let i = 0; i < q; i++) {
        const [n, k] = readLine().split(' ').map(Number);
        
        console.log(getMaxLessThanK(n, k));
    }
}
```
#

<h2><b> Day 6: JavaScript Dates: </h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

// The days of the week are: "Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"
function getDayName(dateString) {
    let dayName;
    // Write your code here
    var day_names = ["Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"]

    var date = new Date(dateString);
    dayName = day_names[date.getDay()];
    return dayName;
}


function main() {
    const d = +(readLine());
    
    for (let i = 0; i < d; i++) {
        const date = readLine();
        
        console.log(getDayName(date));
    }
}

```
#

<h2><b> Day 7: Regular Expressions I: </h2></b>

```

'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

function regexVar() {
    /*
     * Declare a RegExp object variable named 're'
     * It must match a string that starts and ends with the same vowel (i.e., {a, e, i, o, u})
     */
    var re = RegExp(/^([aeiou]).*\1$/);
    
    /*
     * Do not remove the return statement
     */
    return re;
}


function main() {
    const re = regexVar();
    const s = readLine();
    
    console.log(re.test(s));
}
```
#

<h2><b>Day 7: Regular Expressions II: </h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

function regexVar() {
    /*
     * Declare a RegExp object variable named 're'
     * It must match a string that starts with 'Mr.', 'Mrs.', 'Ms.', 'Dr.', or 'Er.', 
     * followed by one or more letters.
     */
    var re = (/^(Mr\.|Dr\.|Er\.|Ms\.|Mrs\.)\s?[a-z|A-Z]+$/);
    
    /*
     * Do not remove the return statement
     */
    return re;
}


function main() {
    const re = regexVar();
    const s = readLine();
    
    console.log(!!s.match(re));
}
```

#

<h2><b> Day 7: Regular Expressions III:</h2></b>

```
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

function regexVar() {
    /*
     * Declare a RegExp object variable named 're'
     * It must match ALL occurrences of numbers in a string.
     */
    
    var re = RegExp('\\d+', 'g');
    
    /*
     * Do not remove the return statement
     */
    return re;
}
```
#

<h2><b> Day 8: Create a Button: </h2></b>
<h2> index.html </h2>

```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
		<link rel="stylesheet" href="css/button.css" type="text/css">
        <title>Button</title>
    </head>
    <body>
		<button class="button" id="btn">0</button> 
		<script src="js/button.js" type="text/javascript"></script>
    </body>
</html>
```

<h2> button.css </h2>

```
button.css:

.button {
    width: 96px;
    height: 48px;
    font-size: 24px;
}
```

<h2>button.js</h2>

```
var btn = document.getElementById("btn");
	btn.addEventListener("click",function() {
		var current_value = this.innerHTML;
		this.innerHTML = parseInt(current_value)+1;
	});
```

#

<h2><b> Day 9 Binary Calculator: </h2></b>
<h2>index.html</h2>

```
<!DOCTYPE html>

<html>

    <head>

        <meta charset="utf-8">

        <link rel="stylesheet" href="css/binaryCalculator.css" type="text/css">

        <title>Binary Calculator</title>

    </head>

    <body> 

        <div id ="res" class="resultClass"> </div>

        <div id="btns" class="buttonContainer">

            <button id="btn0" class="buttonClass"> 0 </button>

            <button id="btn1" class="buttonClass"> 1 </button>

            <button id="btnClr" class="buttonClass"> C </button>

            <button id="btnEql" class="buttonClass"> = </button>

            <button id="btnSum" class="buttonClass"> + </button>

            <button id="btnSub" class="buttonClass"> - </button>

            <button id="btnMul" class="buttonClass"> * </button>

            <button id="btnDiv" class="buttonClass"> / </button>

        </div>    

        <script src="js/binaryCalculator.js" type="text/javascript"></script>

    </body>

</html>

```

<h2> binarycalculator.css</h2>

```
body {
    width: 33%;
}

#res {
    background-color: lightgray;
    border: solid;
    height: 48px;
    font-size: 20px;
}

#btn0, #btn1 {
    background-color: lightgreen;
    color: brown;
}

#btnClr, #btnEql {
    background-color: darkgreen;
    color: white;
}

#btnSum, #btnSub, #btnMul, #btnDiv {
    background-color: black;
    color: red;
}

.buttonClass {
    width: 25%;
    height: 36px;
    font-size: 18px;
    margin: 0px;
    float: left;
}
```
#
<h2><b>Found This Repo Helpful?<br> Consider To Give Me A Treat <br>👇👇👇</b></h2>
<a href="https://www.buymeacoffee.com/r3dhulk"> <img align="center" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="50" width="210" alt="https://www.buymeacoffee.com/r3dhulk" /></a><br><br>
