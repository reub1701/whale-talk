# whale-talk
Codecademy Project utilizing 'for' loops and arrays.

The objective of the project is to compare the elements of 2 strings to translate into "Whale" language consisting only of vowels. Letters 'e' and 'u' are always doubled.  Basically, the code omits all consanants and prints the vowels, doubling up on the e's and u's. 

const input = "The spice must flow.";
const vowels = ['A', 'E', 'I', 'O', 'U'];
const resultArray = [];
for (let i = 0; i < input.length; i++){ 
   for (let v = 0; v < vowels.length; v++){
      if (input[i].toUpperCase() === vowels[v]){
        resultArray.push(vowels[v]);  
        if (vowels[v] === 'E'){
           resultArray.push(vowels[v]);          
        } else if (vowels[v] === 'U') {
          resultArray.push(vowels[v]);
        } 
      }         
   }
};
console.log(resultArray.join("")); 
//Prints: EEIEEUUO
