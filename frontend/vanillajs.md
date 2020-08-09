# Most used #
```javascript
// Add load event when the window is loaded
window.addEventListener('load', (event) => { });
```

# Quick Tips #
```javascript
console.log(obj);
console.table(obj);
console.error(obj); // x icon with red mess
console.info(obj); // i icon
console.assert(1 === 2); // failure can be used for testing
console.clear();
console.dir(obj);
console.group(`${obj.value}`); // helps to log with groups
console.groupEnd(`${obj.value}`); // helps to log with groups
console.count(''); // gives a count of how many times a thing happens

/*
You can have multiple timers if you name them differently. 
You can end a timer by using the timer's name that you started
*/
console.time('fetching data');
console.timeEnd('fetching data'); 
```

# JS Prototypes #
```javascript
Array.prototype.filter()
Array.prototype.map()
Array.prototype.sort()
Array.prototype.reduce()

Array.prototype.some()
Array.prototype.find()
Array.prototype.findIndex()
```


# Example JS Queries #
```javascript
    // find people who are older than 19
    people.some(p => {
        const currentYear = new Date();
        return (currentYear.getFullYear() -  p.year) >= 19;
    });
    
    // are allpeople older than 19?
    people.every(p => {
        const currentYear = new Date();
        return (currentYear.getFullYear() -  p.year) >= 19;
    });
    
    // remove comment index with the id of 823423 from out comment array
    const index = comments.find(x=>{return x.id === 823423});
    comments.splice(index, 1);
    console.log(comments);
```

# Resources #
https://courses.wesbos.com/account
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference