# Lesson Notes

# Array-Cardio-1
Going over Javascript fundamentals

.filter; loops over a function and returns specific value
.map; takes an input and returns same lenght of array
.sort; compares two items to find which of them has a greater value
.reduce; gives a total of instances in an array

Return x value from a site
const category = document.querySelector('.mwcategory')
const links = Array.from(category.querySelectorAll('a')) //selects all links on a page and returns an array of what we need

const de = links
            .map(link => link.textContent)
            .filter(streeName => stretName.includes('de'))
            

Sort in Alphabetical order
const alpha = people.sort(function(lastOne, nextOne)) {
const [aLast, aFirst] = lastOne.split(', ') //put items as separate variables, the split separates the first name from last name at the point where there is a comma 
const [bLast, bFirst] = nextOne.spli(', ')
if (aLast > bLast) {
return 1
}else return -1
}

Count number of instances
const instances = data.reduce(function(obj, item)) {
if (!obj[item]) {
obj[item] = 0      //to check if there is the item in the first place
}
obj[item]++        //increment if the item is present
return obj
}, {}

# Array Cardio 2
Going further into array methods

.some; checks the array to see if at least one member meets the search requirements.
//checking if at least one member is 19 years old//
const isAdult = people.some(function(person) {
const currentYear = (new Date()).getFullYear();
if(currentYear - person.Year >= 19) {
return true
}
})

.every; checks if every single item in the array meets the search requirements.
//To code this, replace .some with .every in the .some function above.

.find; acts like .filter but in this case returns the first ite t finds only.

.findIndex; Finds the location of an item in the array.



# Konami Code
This is something done in Javascript to triger an action when a certain key combination is pressed. It involves creating and array of characters, converting them into a string variable nd assigning it to run with the function. 

Step 1; Create const
const combination = []  //an empty array to contain the key combinations
const secretCode = "change"  //the string that activates the function

window.addEventListener('keyup', (e) => {
combination.push(e.key)  //this adds the pressed key to the end of the array
combination.splice(-secretCode.length - 1, combination.length - secretCode.length)  //limits the number of characters in the array to the number of characters contained in the secret code

if(combination.join('').includes(secretCode)) {      //arr.join converts the array elements into a string

}
} )

//The if statement instructs the function to do a particular thing when it detects the secret code.
