# kontonummer.js
Kontonummer.js är ett bibliotek för att kontroller och validera svenska bankkontonummer. Biblioteket kan användas för att ta reda på vilken bank ett kontonummer tillhör, samt om kontonumret valideras som giltigt enligt stanadrd.

Målsättningen är att stödja samtliga banker vilka är verksamma i Sverige. För närvarande stöds följande banker:
* Amfa Bank
* Avanza Bank
* BlueStep Finans
* BNP
* Citibank
* Danske Bank
* DnB Bank
* Ekobanken
* Erik Penser Bankaktiebolag
* Forex Bank
* Handelsbanken
* ICA Banken
* IKANO Banken
* JAK Medlemsbank
* Landshypotek
* Lån och Spar Bank Sverige
* Länsförsäkringar Bank
* Marginalen Bank
* Nordax Bank
* Nordea
* Nordnet Bank
* Resurs Bank
* Royal Bank of Scotland
* SantanderConsumer Bank
* SBAB
* SEB
* Skandiabanken
* Sparbanken Syd
* Swedbank
* Ålandsbanken
 
# Demo
Ett demo finns tillgängligt här: [http://jop.io/projects/kontonummer-js](http://jop.io/projects/kontonummer-js)

# Installation
```javascript
<script src="kontonummer.min.js"></script>
```

# Användning
```javascript
var result = kontonummer('9420, 417 23 85');
console.log(result);

/* Skriver ut följande objekt till konsolen:

{
  bank_name: "Forex Bank",
  account_type: "Bankkonto", 
  clearing_number: "9420", 
  account_number: "4172385"
}
*/
```
```javascript
var result = kontonummer('123456789');
console.log(result); // false
```

