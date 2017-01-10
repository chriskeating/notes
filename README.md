
var foo = { 'alpha' : 'puffin', 'beta' : 'beagle' };
var keys = Object.keys(foo); 
// would print ['alpha', 'beta']

Access multiple nested keys using
first.hobbies[0]

alert (“Thanks for your input!”);

var name = “Chris”;

then 

name = ckeating

because the var name has already been declared, so you could also do

var nationality;
nationality=“US”;
console.log(nationality);

var weight = 220;

weight + 25 shows 245

a number or set of characters starting with a number can’t be used as a variable name
if a number is in quotations, then it can’t do math

var origNum = 5;
var numToBeAdded = 6;
var newNum = origNum + numToBeAdded;

var origNum = 90;
origNum = origNum + 10;

variable names are case sensitive 

var c = a + b;

% modulus operator 

num++ = num = num + 1;

WEIRD 

var num = 1;
var newNum = num++; 
newNum will be 1 and num will be 2 because the ++ doesn’t come until after newNum has been declared so this is basically another way of writing
var num = 1;
var newNum = num++;
num++;

= is reserved for assigning a value to a variable
== means they can be different value types but are equal
=== means they are exactly the same


!== is not equal to

&& is and in English 

if (weight > 300 && time < 6) {
	alert (“Come to our tryout!”);
}
else { 
	alert (“come to our cookout!”);
}


|| is or in English

also can use parens to group both && and || statements

var cities = [“Atlanta”, “Baltimore”, “Chicago”, “Dallas”];
alert(“ welcome to “ + cities [ 3]);


var pets = [];

pets [0] = “dog”; 
pets [1] = “cat”;
pets [2] = “bird”;
 

pets.pop ();
 allows to remove last element of an array

you can also assign the deleted last element to a variable such as 
var lastElement = pets.pop ();

you can also add to an array using
pets.push (“fish”, “ferret”);

var cities = [" Atlanta", "Baltimore", "Chicago", "Denver", "Los Angeles", "Seattle"];
alert(" Welcome to " + cities[ 3]);

pets.shift (); removes the first entry 

pets unshift (); adds one or more elements to the beginning of an array

pets.splice (2, 2, “pig”, “duck”, “emu” );
first digit is posiiton of where you want to start adding and deleting
second digit is number of existing elements to remove, starting with the first element that comes after the elements that you are splicing in 

var noPets = pets.slice (2, 4); allows you to copy one or more consecutive elements in any position and put them into a new array
first digit is the index of the first digit to be copied
second digit is the index of the element after the last element to be copied

for loops

for (var i = 0; i <=4; i++) {
	if cityToCheck === cleanestCities [i]) {
		alert. 

for (var i = 0;  i <=4 ; i++) {
	if myTeam = top5Team  [i] ) {
		alert (myTeam + “ is a top five team in the country.”);
	}
}


for loop: 

for ( var i = 0; i <= 4; i++)
first statement sets starting value
second statement defines the limit on the loop and remember the way that the array items are indexed (starting with 0,1..
third statement is what to do with the loop after its been run once

a flag is a variable that starts with a default value but the value changes under certain conditions that are defined by the user

var yesTopFive = false;
for (var i = 0; i <= 5; i++ ) {
	if (myTeam === top5Team [i]); {
		yesTopFive = true;
		alert (“Your team is top five in the country”); 
	}
}
if (yesTopFive === false ) {
		alert (“You suck”);
} 

var found = false;

for (var i = 0; i <= 4; i++) {
	if (myCity === topFiveCities [i]) { 
		found = true;
		alert (“Your city was found”);
	}
}
if (found === false) {
	alert (“your city was not found’);
}

var TopFive$$ = false;
for (var i = 0; i <= 6, i++) { 
	if (myTeam === yesTopFive [i]) {
		TopFive$$ = true;
		alert (“get that $$”);
	}
}
if (TopFive$$ === false ) {
	alert (“I have no money”);
} 

keyword break
just put it after the alert instruction (so before the loop runs again) and it’ll stop after the answer has been found		

also, instead of putting a random number in the for loop and hoping it works, we can instead use cleanestCities.length 
NOTE: since cleanestCities.length is 1-based and i is 0-based, we need to stop one short of the length, which is we put the < symbol

alright getting into some next level shit here

got 
First names : Chris Manny Kiko
Last names: Keating Davila, Ayscue
and want to find all possible names

var firstName = [“Chris”, “Manny”, “Kiko”];
var lastName = [“Keating”, “Davila”, Ayscue”];

var fullNames = [];
for (var i = 0; i < firstNames.length; i++) {
	for (var j = 0;  j < lastName.length; j++) {
		fullNames.push (firstNames [i] + lastNames [j]); 
	}
}





var position = [“a”, “m”, “d”, “g”]
var player = [“keating”, “AJrocco”, “AustinRocco”]

var positionAndPlayer = [];
for (var i = 0; i <= position.length, i++] {
	for (var j = 0; j <= player.length, i++) {
		positionAndPlayer.push = (position [i] + player [j]);
	}
}

var cityToCheck = prompt (“Enter your city”);
cityToCheck = cityToCheck.toLowerCase ();
var cleanestCities = [“cheyenne”, “santa fe”..etc];

for (var i = 0; i <= cleanestCities.length; i++)
	if (cityToCheck === cleanestCities [i]) {
		alert (“it’s one of the cleanest cities”);
	}
}
toLowerCase MUST be in camelCase
there is also toUpperCase for weirdos

to copy a section of 

var firstChar = cityToCheck.slice (0,1);
strings are indexed like arrays so 0, 1, 2

var firstChar = cityToCheck.slice (0,1);
var theRest = cityToCheck (1)
firstChar = firstChar.toUpperCase ();
theRest = theRest.toLowerCase ();
var finalWord = firstChar + theRest;

var month = prompt (“What month born?”);
var charsInMonth = month.length; 
if (charsInMonth > 3) {
	monthAbbrev = month.slice (0,3);
}


var str + prompt (“Enter text”);
var numChars = str.length
for (var i = 0; i <numChars; i++) { 
	if (str.slice (




var ww2 = “World War II”;
var text = “XXX”
for (var i = 0; i < text.length; i++) {
	if (text.slice ( i, i + 12) === “World War II”) { 
		text = text.slice (0, i) + “the Second World War” + text.slice (i + 12);
	}
}

indexOf means to take the index of the first character of a specific quoted phrase
so if we are looking for WW2, then use 
var firstChar = text.indexOf (“World War II”);
	if (firstChar !== -1) {
		text = text.slice (0, firstChar) + “the Second WW” + text.slice (firstChar + 12);
	}

however, indexOf only helps us to find the first instance of that shit, so we could loop it if we’re feeling jiggy
lastIndexOf to find the last instance of something in a text

within quotes, spaces can be treated the same as characters

var firstName
var firstChar = firstName.slice (0,1);

var firstChar = firstName.charAt (0);
var lastChar = firstName.charAt (firstName.length - 1); 

for ( var i = 0; i < text.length; i++) {
	if ( text.charAt (i)  === “!”) {
		alert (“excl found”);
		break ;
	}
}

var newText = text.replace (“WW2”, “2nd world war”) but thats only one instance

text.replace (/World War II/g, “second ww”); is global
 

var current = prompt (“Enter current age”);
var ageNextYear = current + 1; //would become 221, not 23

we solve this by using
var currentAge = prompt (“Enter current age”);
var qualifyingAge = parseInt (currentAge) + 1;
this makes what was originally a string into an integer, but it basically just deletes the decimal, so parseInt (“1.99”) becomes 1
what we can use it parseFloat (“1.99”) and that’ll return 1.99
you can also use var integerString = “24”;
var num = Number (integerString);

and then you can convert back using .toString (); so you would put
var numberAsNumber.toString (); which then makes it a string

controlling the length of decimals
something is $9.95, sales tax is 6.5% but we don’t want a huge decimal, so we get 

var totalPrice = listPrice + (listPrice * tax);
totalPrice = total.toFixed (2); //for the number of decimals
var totalPriceWith$ = “$” + totalPrice;

var xx = new Date (); // this creates a date object, but it will not be treated as an a string


var rightNow = new Date ();
var theDay = rightNow.getDay (); 0 is Sunday, 1 is Monday, etc

var dayNames = [“Sun”, “Mon”, “Tues”…];
var now = new Date ();
var theDay = now.getDay ();
var nameOfToday = dayNames [theDay];

a list of time extraction lexicon:

getDay (); day of week
getMonth (); Jan is 1 
getDate (); day of Month
getFullYear ();
getHours (); 0 is midnight, 12 is noon, 23 is 11 pm
getMinutes ();
getSeconds ();
getMilliseconds ();
getTime(); is milliseconds since midnight Jan 1, 1970;

var today = new Date ();
var doomsDay = new Date (“June 20, 2035”);

var msToday = today.getTime (); //in order to get milliseconds for the day
var msDoomsday.getTime (); //and then find the difference
var msDiff = msDoomsday - msToday; //then convert to days
var dDiff = msDIff / (1000 * 60 * 60 * 24);

function addBinary(a,b) {
  var sumNum = a + b;
  var sumNumBinary = '';
  while (sumNum > 1) {
    sumNumBinary.push ('1');
    sumNum -= 2;
  }
  if (sumNum === 1) {
  sumNumBinary.push('1');
  } else if (sumNum === 0){
  sumNumBinary.push('0');
  }
  return sumNumBinary;
}

addBinary (5,7);

Var square = function (x) {
Return x * x;
};

var power = function (base, exponent) {
var result = 1;
for (var count  = 0; count < exponent; count++) {
	result = result * base;
return result;
}
};


function DNAStrand(dna){
  var DNAOtherSide = [];
  for (var i = 0; i < dna.length; i++) {
    if (dna[i] === "A") {
      DNAOtherSide.push("T");
    } else if (dna[i] === T) {
      DNAOtherSide.push("A");
    } else if (dna[i] === C) {
      DNAOtherSide.push("G");
    } else if (dna[i] === G) {
      DNAOtherSide.push("C");
    }
  }
 return DNAOtherSide; 
};  

/*var cashRegister = {
    total:0,
    add: function(itemCost){
        this.total += itemCost;
    }
};

*/


//call the add method for our items
var cashRegister = {
    total: 0,
    add: function (itemCost) {
        this.total += itemCost;
    }
};
/*var eggs = .98;
var milk = 1.23;
var mag = 4.99;
var choc = .45;
cashRegister.add(eggs);
cashRegister.add(milk);
cashRegister.add(mag);
cashRegister.add(choc);
*/
function list (name, price) {
    var name = price;
};
var groceries = new list () {
    eggs: .98,
    milk: 1.23,
    mag: 4.99,
    choc: .45
}; 

for (var i = 0; i <groceries.length; i++) {
    cashRegister.add(groceries[i]);
};
/*
function foodPrices (number) {
    foodPrices.eggs: .98;
    foodPrices.milk: 1.23;
    foodPrices.mag: 4.99;
    foodPrices.choc: .45;
}    
for (var i = 0; i < foodPrices.length; i++) {
    cashRegister.add (foodPrices[i]);*/
//Show the total bill
console.log('Your bill is '+cashRegister.total);





/*var foodAndPrices = [["eggs", "milk", "mags", "choc"],[.98, 1.23, 4.99, .45]]
function respective (foodAndPrices) {
    for (var i = 0; i < foodAndPrices.length; i++) {
        return foodAndPrices [[i],[i]];
    };
};
*/

element is a piece of data in an array

var userChoice = prompt("Do you choose rock, paper or scissors?");
var computerChoice = Math.random();
if (computerChoice < 0.34) {
	computerChoice = "rock";
} else if(computerChoice <= 0.67) {
	computerChoice = "paper";
} else {
	computerChoice = "scissors";
} console.log("Computer: " + computerChoice);

function compare (choice1, choice2) {
    if (choice1 === choice2) {
    return "The result is a tie!";
    } else if (choice1 === "rock") {
        if (choice2 === "paper") {
            return "paper wins";
        } else {
            return "rock wins";
        }
    } else if (choice1 === "paper") {
        if (choice2 === "rock") {
            return "paper wins";
        } else {
            return "scissors win";
        }
    } else if (choice1 === "scissors") {
        if (choice2 === "rock") {
            return "rock wins";
        } else {
            return "scissors win";
        }
    }
};
console.log(compare(userChoice,computerChoice));\

1 is true and 0 is false

_______
var bob = {
    firstName: "Bob",
    lastName: "Jones",
    phoneNumber: "(650) 777-7777",
    email: "bob.jones@example.com"
};

var mary = {
    firstName: "Mary",
    lastName: "Johnson",
    phoneNumber: "(650) 888-8888",
    email: "mary.johnson@example.com"
};

var contacts = [bob, mary];

function printPerson(person) {
    console.log(person.firstName + " " + person.lastName);
}

function list() {
	var contactsLength = contacts.length;
	for (var i = 0; i < contactsLength; i++) {
		printPerson(contacts[i]);
	}
}

/*Create a search function
then call it passing "Jones"*/
function search (lastName) {
    for (var i = 0; i < contacts.length; i++) {
        if (contacts[i].lastName === lastName) {
            printPerson(contacts[i]);
        }
    }
};
search ("Jones");

method is a function associated with a specific object

function transformEmployeeData(array) {
    var answer = [];
    for (var i = 0; i < array.length; i++) {
        var miniObject = {};
        for (var j = 0; j < array[i].length; j++) {
            var miniAnswer;
            miniAnswer += (array[i][j][0] + ": " + array[i][j][1]);
        }
        answer.push({miniAnswer});
        miniAnswer = 0;
    }
    return answer;
}
        
/* for loop that goes through the indexes of each and adds to an object using either literal notation or a constructor
potentially 3 for loops embedded inside one another
*/



for (var i = 0; i < customerData.length; i++) {
        if (customerData[i][0] === 0) {
            greeting = 'Welcome! Is this your first time?';
        } else if (customerData[i][0] === 1) {
            greeting = "Welcome back, Joe! We're glad you liked us the first time!";
        } else if (customerData[i][0] > 1) {
            greeting = "Welcome back, Carol! So glad to see you again!";

function assertEqual (actual, expected, testName) {
  if (actual === expected) {
    console.log('passed');
  } else {
    console.log('FAILED: ' + testName + '. Expected: ' + expected + ' but got ' + actual);
  }
}


function assertEqual(actual, expected, testName) {
  if (actual === expected) {
    console.log('passed');
  } else {
    console.log('FAILED ' + testName + ': Expected ' + expected + ', but got ' + actual);
  }
}

function assertEqual (actual, expected, testName) {
  if (actual === expected) {
    console.log('passed')';
  } else {
    console.log('FAILED ' + testName + ': Expected ' + expected + ', but got ' + actual);
  }
}

App Academy Exercises, My Solutions

/*disemvowel

Write a function disemvowel(string), which takes in a string, and returns that string with all the vowels removed. Treat "y" as a consonant.*/

function disemvowel(string) {
  var newString = '';
  for (var i = string.length - 1; i >= 0; i--) {
    if (string[i] === 'a' || string[i] === 'e' || string[i] === 'i' || string[i] === 'o' || string[i] === 'u') {
      string = string.substr(0,i) + string.substr(i+1);
    }
  }
  return string;
}

disemvowel("foobar");// == "fbr"
disemvowel("ruby");// == "rby"xz
//disemvowel("aeiou");// == ""

__
function minsToHoursAndMins (mins) {
  var hours = Math.floor (mins/60);
  var minutes = mins % 60;
  var minutesString = ('00' + minutes).slice(-2)
  var hourAndMin = hours + ':' + minutesString;
  return hourAndMin;
}

minsToHoursAndMins(65)

function positionsOfTwoNumsThatSumToZero (array) {
  var positionArray = [];
  for (var i = 0; i < array.length; i++) {
    if (array[i] === 0) {
      positionArray.push(i,i);
      return positionArray;
    } else {
      for (var j = 0; j < array.length; j++) {
        if (array[i] + array[j] === 0) {
          positionArray.push(i,j);
          return positionArray;
        }
      }
    }
  }
  return null;
}
positionsOfTwoNumsThatSumToZero([1,2,3,-2])

___
function returnThirdGreatestNum (array) {
  var orderMostToLeast012 = array[0] > array[1] && array[1] > array[2];
  var orderMostToLeast021 = array[0] > array[2] && array[2] > array[1];
  var orderMostToLeast102 = array[1] > array[0] && array[0] > array[2];
  var orderMostToLeast120 = array[1] > array[2] && array[2] > array[0];
  var orderMostToLeast201 = array[2] > array[0] && array[0] > array[1];
  var orderMostToLeast210 = array[2] > array[1] && array[1] > array[0];
  switch ()
}

function returnMostCommonLetterAndCount (string) {
  var mostCommonLetter = '';
  var count = 0;
  var obj = {};
  for (var i = 0; i < string.length; i++) {
    if (obj.hasOwnProperty(string[i])) {
      obj[string[i]]++;
    } else {
      obj[string[i]] = 1;
    }
  }
  var highestCount = 0;
  var character;
  for (var key in obj) {
    if (obj[key] > highestCount) {
      highestCount = obj[key];
      character = key;
    }
  }
  var arrayContainingAnswer = [];
  arrayContainingAnswer.push(character, highestCount);
  return arrayContainingAnswer;
}

/*# Write a method that takes in a string. Your method should return the
# most common letter in the array, and a count of how many times it
# appears.
#
# Difficulty: medium.*/

function returnMostCommonLetterAndCount (string) {
  var mostCommonLetter = '';
  var count = 0;
  var obj = {};
  for (var i = 0; i < string.length; i++) {
    if (obj.hasOwnProperty(string[i])) {
      obj[string[i]]++;
    } else {
      obj[string[i]] = 1;
    }
  }
  var highestCount = 0;
  var character;
  for (var key in obj) {
    if (obj[key] > highestCount) {
      highestCount = obj[key];
      character = key;
    }
  }
  var arrayContainingAnswer = [];
  arrayContainingAnswer.push(character, highestCount);
  return arrayContainingAnswer;
}

returnMostCommonLetterAndCount('abcaabbb');
/*
# These are tests to check that your code is working. After writing
# your solution, they should all print true.

puts(
  'most_common_letter("abca") == ["a", 2]: ' +
  (most_common_letter('abca') == ['a', 2]).to_s
)
puts(
  'most_common_letter("abbab") == ["b", 3]: ' +
  (most_common_letter('abbab') == ['b', 3]).to_s
)
*/

function numberToStringWithDashesAroundOddNumbers (num) {
  var numToString = num.toString();
  var stringWithDashes = '';
  for (var i = 0; i < numToString.length; i++) {
    if (numToString[i] % 2 === 1) {
      stringWithDashes += '-' + numToString[i] + '-';
    } else {
      stringWithDashes += numToString[i];
    }
  }
  for (var j = 0; j < stringWithDashes.length; j++) {
    if ((stringWithDashes[j] === '-') && (stringWithDashes[j+1] === '-')) {
      stringWithDashes = stringWithDashes.substr(0,j) + stringWithDashes.substr(j+1);
    }
  }
  if (stringWithDashes[0] === '-') {
    stringWithDashes = stringWithDashes.substr(1);
  }
  if (stringWithDashes[stringWithDashes.length - 1] === '-') {
    stringWithDashes = stringWithDashes.substr(0,stringWithDashes.length - 1);
  }
  return stringWithDashes;
}
function capitalizeFirstLetterOfAllWords(string) {
  var splitString = string.split(' ');
  var firstLetterCapitalizedArray = [];
  for (var i = 0; i < splitString.length; i++) {
    firstLetterCapitalizedArray.push(splitString[i][0].toUpperCase() + splitString[i].substr(1));
  }
  var capitalizedSentence = firstLetterCapitalizedArray.join();
  var capitalizedSentenceWithSpace = capitalizedSentence.replace(/,/g, ' ')
  return capitalizedSentenceWithSpace;
}

capitalizeFirstLetterOfAllWords('a whole new world');

function returnNthPrimeNum (n) {
function returnTrueIfPrime (num) {
  var isPrime = true;
  var primeNumArray = [];
  for (var i = 2; i < num; i++) {
    var result = num % i;
     if (result === 0) {
       isPrime = false;
       return isPrime;
     } 
  }
  return isPrime;
}
var count = 0;
var number = 1;
while (count < n) {
  number++;
  if (returnTrueIfPrime(number) === true) {
    count++;
  }
}
return number;
}

returnNthPrimeNum(1);//2
returnNthPrimeNum(2);//3
returnNthPrimeNum(3);//5
returnNthPrimeNum(4);//7
returnNthPrimeNum(5);//11

__

function returnGreatestCommonFactor(num1,num2) {
  if (num1 % num2 === 0) {
    return num2;
  } else if (num2 % num1 === 0) {
    return num1;
  }
  var GCF = 1;
  if (num1 > num2) {
    for (var i = 2; i < num2; i++) {
      if (num1 % i === 0 && num2 % i === 0) {
        GCF = i;
      }
    }
  } else {
    for (var j = 2; j < num1; j++) {
      if (num1 % j === 0 && num2 % j === 0) {
        GCF = j;
      }
    }
  }
  return GCF;
}
returnGreatestCommonFactor(16,24)

____

function offsetStringUsingInteger (int,string) {
  while (int > 26) {
    int -= 26;
  }
  if (int === 26) {
    return string;
  }
  var returnString = '';
  for (var i = 0; i < string.length; i++) {
    if (string[i] === ' ') {
      returnString += ' ';
    } else {
      var shiftedNum = string.charCodeAt(i) + int;
      if (shiftedNum > 122) {
        shiftedNum = shiftedNum - 26;
      }
      var shiftedLetter = String.fromCharCode(shiftedNum);
      returnString = returnString + shiftedLetter;
    }
    
  }
  
  return returnString;
}
offsetStringUsingInteger(3,'abc');
offsetStringUsingInteger(3,'abc xyz');
