# Array-Cardio-1
Going over Javascript fundamentals

.filter; loops a function and returns specific value
.map; takes an input and returns same lenght of array
.sort; compares two items to find whih of hem ha a greater value
.reduce; gives a total of instances in an array

Return x value from a site
const category = document.querySelector('.mwcategory')
const links = Array.from(category.querySelectorAll('a')) //select all links on a page and returns an array of what we need

const de = links
            .map(link => link.textContent)
            .filter(streeName => stretName.includes('de'))
            

Sort in Alphabetical order
const alpha = people.sort(function(lastOne, nextOne)) {
const [aLast, aFirst] = lastOne.split(', ') //put items as separate variables, the split separates the first name from, last name at the point where there is a comma 
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
