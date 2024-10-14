# ArraysandLoops
Arrays and Loops

// Sum of Resistors in Series
function sumaDeResitancia(resistors) {
   
    const total = resistors.reduce((acc, curr) => acc + Math.abs(curr), 0);
    return ${total} ohms;
}

console.log(sumaDeResitance([-1,5,6,3])); // "15 ohms"
console.log(sumaDeResitance([14,3.5,6])); // "23.5 ohms"
console.log(sumaDeResitance([8,15,100])); // "123 ohms"


// Secret Society

function secretSociety(names) {
 
    return names.map(name => name[0]).sort().join('');
}
console.log(secretSociety(["Esperanza", "Franco", "Nia"]));
console.log(secretSociety(['Phoebe', 'Ross', 'Chandler', 'Joey', 'Monica', 'Rachel']));
console.log(secretSociety(['Harry', 'Ron', 'Hermione'])); 


// Array of Multiples

function arrayMultiplos(num, len) {
 
    return Array.from({ length: len }, (_, i) => num * (i + 1));
}
console.log(arrayMultiplos(3, 8)); 
console.log(arrayMultiplos(5, 7)); 
