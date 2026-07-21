1. Create Employee, Mobile and Car Objects

Objects are used to store data in the form of key-value pairs.

let employee = {
  name: "Rahul",
  age: 25,
  department: "IT"
};

let mobile = {
  brand: "Samsung",
  model: "S24",
  price: 70000
};

let car = {
  brand: "Toyota",
  model: "Fortuner",
  color: "Black"
};

Explanation:
Here, Employee, Mobile, and Car are objects containing different properties and values.



2. Add, Update and Delete Properties
employee.salary = 50000;      // Add
employee.age = 26;            // Update
delete employee.department;   // Delete

Explanation:

New properties can be added using . notation.
Existing values can be modified.
delete removes a property from an object.



3. Loop Through an Object's Properties
for(let key in employee){
  console.log(key, employee[key]);
}

Explanation:
The for...in loop is used to access all properties of an object one by one.



4. Create an Array of 5 Students
let students = [
  {name: "Rahul", marks: 85},
  {name: "Priya", marks: 92},
  {name: "Aman", marks: 76},
  {name: "Neha", marks: 88},
  {name: "Riya", marks: 95}
];



Explanation:
This is an array containing five student objects.



5. Use map() to Get Their Names
let names = students.map(student => student.name);

console.log(names);

Output:

["Rahul", "Priya", "Aman", "Neha", "Riya"]

Explanation:
map() creates a new array by extracting the names from each student object.



6. Use filter() to Get Students Above 80 Marks
let topStudents = students.filter(student => student.marks > 80);

console.log(topStudents);

Explanation:
filter() returns only those students whose marks are greater than 80.



7. Use find() to Search for One Student
let student = students.find(student => student.name === "Neha");

console.log(student);

Explanation:
find() returns the first matching student object.



8. Use reduce() to Calculate Total Marks
let total = students.reduce(
  (sum, student) => sum + student.marks,
  0
);

console.log(total);

Output:

436

Explanation:
reduce() combines all marks into a single total value.



9. Sort the Students by Marks
students.sort((a, b) => a.marks - b.marks);

console.log(students);

Explanation:
sort() arranges students in ascending order according to their marks.

For descending order:

students.sort((a, b) => b.marks - a.marks);