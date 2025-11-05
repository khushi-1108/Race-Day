# Race-Day
JavaScript practice project from Codecademy demonstrating conditionals and logical operators.

This project is part of Codecademy’s **JavaScript conditionals** lesson. It assigns a race time to runners based on their age and registration status.

---

## 💻 How It Works
- Generates a random race number using `Math.random()`
- Checks if the runner registered early and their age
- Prints different race times based on the conditions

---

## 🧩 Example Code
```js
let raceNumber = Math.floor(Math.random() * 1000);

let registeredEarly = false; 
let age = 18;

if (registeredEarly && age > 18){
  raceNumber += 1000;
}
if (registeredEarly && age > 18){
  console.log(`Your race will start at 9:30 am runner number ${raceNumber}.`);
} else if (registeredEarly || age > 18){
  console.log(`${raceNumber} will start race at 11:00am`);
} else if (age < 18) {
  console.log(`Your race will start at 12:30 pm runner number ${raceNumber}`);
} else {
  console.log(`See the registration desk`);
}
