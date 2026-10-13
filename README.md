# Learn JavaScript. Interactive tutorial.

Realiza los retos de [learnjavascript.online](https://learnjavascript.online/), una forma de aprender y practicar JavaScript moderno. 
Aprende en un entorno interactivo, con lecciones breves y resolviendo  desafíos directamente en el navegador.
Pega aquí los enunciados y tus soluciones.

Refactoriza el código de manera que sea REALMENTE JavaScript moderno:
- Evita el uso de bucles `for`/`while`
- No uses `var`
- Usa arrow functions. Simplifícalas lo más posible.
- Haz uso de médodos iterativos de arrays `map`, `filter`, `reduce`, `slice`...
- Usa operador ternario
- Usa template literal
- Usa las asignaciones simplificadas `++`, `+=`...

## 1. Basic Functions
### Basic sum
```javascript
function sum(x, y) {
    return x + y;
    console.log("Hello World"); // esto NUNCA se ejecutará
}
```

### Basic multiplication
```javascript
function multiply(a, b) {
    return a * b;
}

```

## 2. Strings I
```javascript
function getCharCount(str) {
    return str.length;
}

function shoutMyName(name) {
    return name.toUpperCase();
}


function lowerName(name) {
    return name.toLowerCase();
}

function getFirstCharacter(name) {
    return name[0];
}

function getLastCharacter(name) {
    return name[name.length - 1];
}

function skipFirstCharacter(text) {
    return text.substring(1);
}

export function getDescription(text) {
    return text.slice(0, 10);
}

function concatInitials(firstNameInitial, lastNameInitial) {
    return firstNameInitial + lastNameInitial;
}

export function getDescription(text) {
    return `${text.slice(0, 10)}...`;
}

function sayHello(name) {
    return `Hello ${name}`;
}

function getFullName(firstName, lastName) {
    return `${firstName} ${lastName}`;
}

function getMultilineString() {
    return `I am learning JavaScript
and I found it to be
quite fun!`;
}

export function renderTableRow(label, value) {
    return `<tr>
    <td>${label}</td>
    <td>${value}</td>
</tr>`;
}

function capitalize(word) {
    return word[0].toUpperCase() + word.slice(1).toLowerCase();
}

# Todo el mismo ejercicio
/** @param {string} name */
export function getNumberOfChars(name) {
    return name.length;
}

/** @param {string} name */
export function getFirstChar(name) {
    return name[0];
}

/** @param {string} name */
export function getLastChar(name) {
    return name[name.length - 1];
}

/** @param {string} name */
export function getLower(name) {
    return name.toLowerCase();
}

/** @param {string} name */
export function getUpper(name) {
    return name.toUpperCase();
}

/** @param {string} name */
export function getCapitalized(name) {
    return name[0].toUpperCase() + name.slice(1).toLowerCase();
}
# Hasta aqui
```
## 3. Numbers
```javascript
function convertNumberToString(number) {
    return number.toString();
}

export function getNextAge(age) {
    return Number(age) + 1;
}

export function getBoxWidth(value) {
    return parseInt(value, 10);
}

export function getDivisionRemainderBy2(number) {
    return number % 2;
}
```
## 4. Variables
```javascript
let count = 0;
count++;

const ageLimit = 18;
```

## 5. Conditions
```javascript
function canVote(age) {
    return age >= 18;
}

export function getNextAge(age) {
    if (age === "") {
        return 0;
    }
    return Number(age) + 1;
}

export function getDescription(text) {
    if (text.length > 10) {
        return text.slice(0, 10) + "...";
    }
    return text;
}

function canVote(age) {
    return age >= 18;
}

export function evenOrOdd(number) {
    if (number % 2 === 0) {
        return "even";
    }
    return "odd";
}
```

## 6. Arrays I
```javascript
function getEmptyArray() {
    return [];
}

function getNumberOfElements(elements) {
    return elements.length;
}

function useCalculator(apps) {
    apps.push("Calculator");
    return apps;
}

function useApp(apps, app) {
    apps.push(app);
    return apps;
}

function getFirstApp(apps) {
    return apps[0];
}

function getLastApp(apps) {
    return apps[apps.length - 1];
}

function loopThroughElements(elements) {
    elements.forEach(element => {
        console.log(element);
    });
}

function logUserIds(userIds) {
    userIds.forEach(userId => {
        console.log(userId);
    });
}

function sumGrades(grades) {
    let total = 0;
    grades.forEach(grade => {
        total += grade;
    });
    return total;
}

function sumPositiveNumbers(numbers) {
    let total = 0;
    numbers.forEach(number => {
        if (number > 0) {
            total += number;
        }
    });
    return total;
}

function sumOddNumbers(numbers) {
    let total = 0;
    numbers.forEach(number => {
        if (number % 2 !== 0) {
            total += number;
        }
    });
    return total;
}

export function getDropdown(countries) {
    let html = '<option value="">Please select</option>';
    countries.forEach(country => {
        html += `<option value="${country.toLowerCase()}">${country}</option>`;
    });
    return html;
}

export function renderTableRows(rows) {
    let html = "";
    rows.forEach(row => {
        const label = row[0];
        const value = row[1];
        html += `<tr>
    <td>${label}</td>
    <td>${value}</td>
</tr>`;
    });
    return html;
}
```

## 7. Arrays II & callbacks
```javascript
function getPositiveTemperatures(temperatures) {
    return temperatures.filter(temperature => temperature > 0);
}

function getFreezingTemperatures(temperatures) {
    return temperatures.filter(temperature => temperature < 0);
}

function getYear(years, searchYear) {
    return years.find(year => year === searchYear);
}

function getOddYears(years) {
    return years.filter(year => year % 2 !== 0);
}

function isAppUsed(apps, app) {
    return apps.includes(app);
}

function getStringSizes(strings) {
    return strings.map(string => string.length);
}

# Todo esto es el ejercicio
/** @param {number[]} grades */
export function getNumberOfGrades(grades) {
    return grades.length;
}

/** @param {number[]} grades */
export function getSumGrades(grades) {
    let total = 0;
    grades.forEach(grade => {
        total += grade;
    });
    return total;
}

/** @param {number[]} grades */
export function getAverageValue(grades) {
    if (grades.length === 0) return 0;
    let total = 0;
    grades.forEach(grade => {
        total += grade;
    });
    return total / grades.length;
}

/** @param {number[]} grades */
export function getPassingGrades(grades) {
    return grades.filter(grade => grade >= 10);
}

/** @param {number[]} grades */
export function getFailingGrades(grades) {
    return grades.filter(grade => grade <= 9);
}

/** @param {number[]} grades */
export function getRaisedGrades(grades) {
    return grades.map(grade => {
        const raised = grade + 1;
        return raised > 20 ? 20 : raised;
    });
}
# Hasta aqui

export function getVotersCount(ages) {
    return ages.filter(age => age >= 18).length;
}
```

