//this is comment
var x = 0
var y = 1

var name = "Vimal"

//System.out.println()
console.log(typeof name)


var zip = 35434
console.log(typeof zip)

var trainer = true
console.log(typeof trainer)

var user = {name:"Vimal"}

console.log(typeof user)

var name = 'Mike'

console.log('Hi ' + name)

//Operators
// Arithmetic: + - / * %
// Unary: ++ -- += -= *=
// Assignment: =
// Logical: && ||
// Comparison: < <= > >=
// Ternary: <expression> ? true : false
// Equality: == ===

//Double equals: compares the data alone
//Triple equals: compares the data along with type

var age = 25
var ageString = '25'

console.log(age === ageString)

//Operator Precendence
//(4 - 6) * 3 / 5

//if, if-else
if(true){
  
}
//switch

//Arrays (can grow)
var arr = ['Train','Bus',100,true]
console.log(arr[0])
arr[2] = 'Car'

for(var i = 0; i < arr.length; i++){
  console.log(arr[i])
}

console.log(typeof arr)

//while, do-while
//break, continue


//Methods
//Functions

//void
//returning value

function add(a,b){
  var x = a + b
  return x
}

function print(value) {
  console.log('Result is ' +value)
}

var result = add(5,6)
print(result)

//Objects

function apply () {
    console.log('Applying job...')
  }

var user = {
  name: 'Mike',
  scores: [],
  applyJob: apply,
  address: {
    city: 'St.Louis',
    state: 'MO'
  }
}

console.log(user.name)
console.log(user.address.city)

user.applyJob()

user.name = 'Peter'

console.log(user.name)

user.email = 'peter@testemail.com'

console.log(user)

var fruits = 'Apple,Banana,Grapes'
var arr = fruits.split(',')


//function - regular
//function - callback

function add (a,b, cbFn) {
//  return a + b
  setTimeout(function(){
    cbFn(a + b)
  },2000)
  //cbFn(a + b)
}

//var result = add(5,6)

add(5,6, function (x){
  console.log('result: '+x)
})


// setTimeout(function() {
//   console.log('Testing')
// }, 2000)

// setInterval(function() {
//   console.log('Testing interval')
// }, 1000)

//later - asynchronous


console.log('B')

function main(){
  print('A')
  
}

function print(value){
  console.log(value)
  
}

setTimeout(function(){
  console.log('C')
},0)

setTimeout(function(){
  console.log('D')
},100)

console.log('E')

main('A')
