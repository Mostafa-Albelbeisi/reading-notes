# Lists and Keys
1- **What does .map() return?** a map object.

2- **If I want to loop through an array and display each value in JSX, how do I do that in React?** using the JavaScript map()function.

3- **Each list item needs a unique** Key.

4- **What is the purpose of a key?** Keys help React identify which items have changed, are added, or are removed.

# Spread 
1- **What is the spread operator?** The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

2- **List 4 things that the spread operator can do.**
- Copying an array.
- Concatenating or combining arrays.
- Using Math functions.
- Using an array as arguments.

 3- **Give an example of using the spread operator to combine two arrays.**

const array1 = [1, 2, 3];

const array2 = [4, 5, 6];

const attemptToMerge = [array1, array];

attemptToMerge;

this is a result [ [1, 2, 3],  [4, 5, 6] ]

4- **Give an example of using the spread operator to add a new item to an array.**

fruits[0] = 'value', then we called in console.lgo

5- **Give an example of using the spread operator to combine two objects into one.**

let person = {

    firstName: 'John',
    lastName: 'Doe',
    age: 25,
    ssn: '123-456-2356'
};


let job = {

    jobTitle: 'JavaScript Developer',
    location: 'USA'
};

let employee = {

    ...person,
    ...job
};

console.log(employee);


# How to Pass Functions between Components
1- **In the video, what is the first step that the developer does to pass functions between components?** Create a function

2- **In your own words, what does the increment function do?** It increases the number in the value you pass through

3- **How can you pass a method from a parent component into a child component?** As prop

4- **How does the child component invoke a method that was passed to it from a parent component?** 

Wrap the Child component in a forwardRef .

Use the useImperativeHandle hook in the child to add a function to the Child .

Call the Child's function from the Parent using the ref, e.g. childRef. current. childFunction() .

## Things I want to know more about
