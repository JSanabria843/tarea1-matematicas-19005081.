# tarea1-matematicas-19005081.
Primera sección
1. Utilice el procedimiento visto en clase para la conversión de los siguientes números
decimales a binarios:
a. 7            7/2 =3 resto 1  3/2=1  resto 1   1/2 = 0  resto  1  

R//     1 1 1 
b. 45         45/2= 22 resto 1      22/2=11 resto 0    11/2 =5  resto 1    5/2 = 2    resto 1  2/2= 1 resto 1   1/2=  0    resto 1     

 R//    101101

c. 123       123/2= 61 resto 1 61/2= 30 resto 1 30/2= 15 resto 1 15/2= 7 resto 1   7/2= 3 resto 1 3/2= 1 resto 1   1/2=0 resto 1      
 R//  1101111

d. 8.75     
Parte entera:  8/2 = 4  resto 0   4/2=2  resto 0    2/2=  0   resto 0   1/2=1  resto 1 
Parte decimal  0.75x2 = 1.5  lueog 0.5 x2 = 1.0  tomamos el primer numero de cada resultado dando este: 11 
R //  1000.11
e. -18 (uAlice complemento a dos, ver un ejemplo en la sección de anexos de este
documento).   1110 1110

Tablas de verdad

A.
https://github.com/JSanabria843/tarea1-matematicas-19005081./issues/1#issue-2631785908

B.
https://github.com/JSanabria843/tarea1-matematicas-19005081./issues/2#issue-2631786979

C.
https://github.com/JSanabria843/tarea1-matematicas-19005081./issues/3#issue-2631787342

D.
https://github.com/JSanabria843/tarea1-matematicas-19005081./issues/4#issue-2631787656

E.
https://github.com/JSanabria843/tarea1-matematicas-19005081./issues/5#issue-2631787998

Ejercicio 1
https://github.com/JSanabria843/tarea1-matematicas-19005081./issues/6#issue-2631789218

function evaluateRisk(income, hasLoans, latePayments, isStudent) {
   
    if ((income < 20000 && latePayments > 3) || (hasLoans && isStudent)) {
        return 'High';
    }
   
    else if ((income >= 20000 && income <= 50000 && latePayments <= 2) || (hasLoans && !isStudent)) {
        return 'Moderate';
    }
   
    else {
        return 'Low';
    }
}

// Ejemplo de uso
console.log(evaluateRisk(15000, true, 4, true));  // "High"
console.log(evaluateRisk(30000, true, 1, false)); // "Moderate"
console.log(evaluateRisk(60000, false, 0, false)); // "Low"



Ejercicio 2:
https://github.com/JSanabria843/tarea1-matematicas-19005081./issues/7#issue-2631790504

function recommendProduct(age, isMember, purchaseHistory) {
    const { tech, fashion, other } = purchaseHistory;

 
    if ((isMember && tech >= 5) || (age >= 18 && age <= 30 && fashion >= 2)) {
        return 'High-Tech Product';
    }
   
    else if ((!isMember && (tech + fashion + other) >= 3) || (age >= 25 && age <= 40)) {
        return 'Fashion Product';
    }
   
    else {
        return 'Generic Product';
    }
}

// Ejemplo de uso


console.log(recommendProduct(22, true, { tech: 6, fashion: 1, other: 2 }));   // "High-Tech Product"
console.log(recommendProduct(28, false, { tech: 1, fashion: 2, other: 1 }));  // "Fashion Product"
console.log(recommendProduct(45, false, { tech: 0, fashion: 0, other: 1 }));  // "Generic Product"



