[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11792667&assignment_repo_type=AssignmentRepo)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];  //If length of a == 1 then return index 0 of array a.
    var foo = mystery(a.slice(1, a.length)) //Recursive call to find next element in the array
    if(foo > a[0]) return foo;  //If foo is larger than index 0 of array a then return foo
    else return a[0];   //If not return a[0]
}

// If the length of the array is 1 then it returns index 0 of the array. Otherwise it will recursively call itself to the array excluding the first element and store the result as foo. It compares foo with the first element in the array and if the result is greater returns the value foo. Else it will return the first element. The mystery function is going through and sorting the array by finding the largest element. 
```
