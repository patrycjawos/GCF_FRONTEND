---
coverY: 0
---

# 1 Podstawy javascript

JavaScript to wszechstronny język programowania stosowany głównie do tworzenia interaktywnych stron internetowych. Jest to język skryptowy, który umożliwia dodawanie funkcjonalności, interakcji i animacji do stron internetowych. Jest także szeroko używany w tworzeniu aplikacji internetowych zarówno po stronie klienta (front-end) jak i serwera (back-end), dzięki platformie Node.js. JavaScript jest dynamiczny, obsługuje wiele paradygmatów programowania (takich jak programowanie obiektowe czy funkcjonalne) i posiada bogate zestaw bibliotek i frameworków ułatwiających rozwój oprogramowania.

### Operatory

JavaScript ma wiele różnych operatorów, które umożliwiają wykonywanie różnych operacji na danych. Oto kilka podstawowych operatorów w JavaScript:

1. **Arytmetyczne operatory:** `+` (dodawanie), `-` (odejmowanie), `*` (mnożenie), `/` (dzielenie), `%` (modulo, reszta z dzielenia).
2. **Przypisania:** `=` (przypisanie wartości do zmiennej), `+=`, `-=` (skrócony zapis dodawania/odejmowania do zmiennej), `*=`, `/=` (skrócony zapis mnożenia/dzielenia zmiennej).
3. **Porównania:** `==` (równy wartości), `===` (równy wartości i typu), `!=` (nierówny wartości), `!==` (nierówny wartości lub typu), `>` (większy niż), `<` (mniejszy niż), `>=` (większy bądź równy), `<=` (mniejszy bądź równy).
4. **Logiczne:** `&&` (i logiczne), `||` (lub logiczne), `!` (negacja logiczna).
5. **Bitowe:** `&` (AND bitowy), `|` (OR bitowy), `^` (XOR bitowy), `~` (NOT bitowy), `<<` (przesunięcie bitowe w lewo), `>>` (przesunięcie bitowe w prawo).
6. **Inne:** `?:` (operator warunkowy - trójargumentowy), `,` (operator przecinka - służy do oddzielenia wyrażeń).

### Typy danych

W JavaScript istnieje kilka podstawowych typów danych, które mogą być wykorzystywane do przechowywania różnych rodzajów informacji. Oto kilka głównych typów danych w JavaScript:

1. **Typy proste (Primitive types):**
   * **String** - ciąg znaków, np. `"Hello World"`.
   * **Number** - liczby, zarówno całkowite jak i zmiennoprzecinkowe, np. `10`, `3.14`.
   * **Boolean** - logiczne wartości `true` lub `false`.
   * **Null** - reprezentuje brak wartości lub pustkę.
   * **Undefined** - oznacza zmienną, która nie została zdefiniowana lub nie ma przypisanej wartości.
   * **Symbol** - wprowadzony w ECMAScript 6, reprezentuje unikalne i niezmiennicze wartości, często używane jako klucze w obiektach.
2. **Typy referencyjne (Reference types):**
   * **Object** - obiekty, które zawierają właściwości (pary klucz-wartość), np. `{ name: 'John', age: 30 }`.
   * **Array** - tablice, które przechowują sekwencje wartości, np. `[1, 2, 3, 4]`.
   * **Function** - funkcje, które są obiektami i mogą być wywoływane, np. `function greet() { console.log("Hello!"); }`.
   * **Date** - obiekt reprezentujący datę i czas.
   * **RegExp** - obiekt reprezentujący wyrażenie regularne do manipulowania tekstami.

JavaScript jest językiem dynamicznym, co oznacza, że zmienne mogą zmieniać typ danych w trakcie działania programu. Jest to często nazywane "luźnym typowaniem" (dynamic typing). Programiści nie muszą jawne deklarować typów zmiennych - typ jest automatycznie przypisywany w trakcie wykonywania kodu.

### Zmienne

Zmienne w JavaScript są tworzone poprzez użycie słowa kluczowego `var`, `let` lub `const`, po którym następuje nazwa zmiennej.

1.  **`var`:** Wcześniej używany sposób deklaracji zmiennych w JavaScript. Zmienna zadeklarowana za pomocą `var` ma zakres funkcji, nie jest ograniczona do bloku kodu.

    ```javascript
    javascriptCopy codevar x = 10;
    ```
2.  **`let`:** Został wprowadzony w nowszych wersjach JavaScript. Zmienna zadeklarowana za pomocą `let` ma zasięg ograniczony do bloku, w którym została zdefiniowana.

    ```javascript
    javascriptCopy codelet y = 20;
    ```
3.  **`const`:** Tworzy stałą, której wartość nie może być zmieniona po zainicjalizowaniu. Także ma zasięg ograniczony do bloku.

    ```javascript
    javascriptCopy codeconst z = 30;
    ```

Aby zainicjalizować zmienną w JavaScript, po słowie kluczowym (`var`, `let`, `const`) podaje się nazwę zmiennej, a następnie używa operatora przypisania `=` do przypisania wartości do zmiennej.

```javascript
javascriptCopy codelet name = 'John';
const age = 25;
```

JavaScript jest językiem dynamicznym, więc typ zmiennej jest automatycznie określany na podstawie przypisanej wartości. Zmienne mogą przechowywać różne typy danych w trakcie działania programu.

### Warunki

W JavaScript instrukcje warunkowe pozwalają na wykonanie różnych bloków kodu w zależności od spełnienia określonych warunków. Podstawowymi instrukcjami warunkowymi są `if`, `else if` i `else`. Oto sposób ich tworzenia:

#### Instrukcja warunkowa `if`:

```javascript
let x = 10;

if (x > 5) {
    console.log("x jest większe niż 5");
}
```

#### Instrukcja warunkowa `if`/`else`:

```javascript
let y = 3;

if (y > 5) {
    console.log("y jest większe niż 5");
} else {
    console.log("y nie jest większe niż 5");
}
```

#### Instrukcja warunkowa `if`/`else if`/`else`:

```javascript
let z = 7;

if (z > 10) {
    console.log("z jest większe niż 10");
} else if (z > 5) {
    console.log("z jest większe niż 5, ale mniejsze niż 10");
} else {
    console.log("z jest mniejsze lub równe 5");
}
```

Można także zagnieżdżać instrukcje warunkowe, czyli umieszczać jedną instrukcję warunkową wewnątrz innej.

#### Przykład zagnieżdżonej instrukcji warunkowej:

```javascript
let a = 30;
let b = 20;

if (a === 30) {
    if (b === 20) {
        console.log("a jest równe 30 i b jest równe 20");
    }
}
```

Instrukcje warunkowe opierają się na ewaluacji wyrażeń logicznych. Warunek musi zwrócić wartość typu logicznego (`true` lub `false`). Jeśli warunek jest prawdziwy (`true`), odpowiedni blok kodu jest wykonywany. W przeciwnym razie wykonywany jest inny blok kodu lub program przechodzi dalej, jeśli nie ma kolejnych warunków.

### Funkcje

Funkcje w JavaScript mogą być tworzone na kilka różnych sposobów. Oto kilka podstawowych sposobów definiowania funkcji:

#### Definicja funkcji za pomocą słowa kluczowego `function`:

```javascript
function greet() {
    console.log("Witaj, świecie!");
}

// Wywołanie funkcji
greet();
```

#### Funkcje z parametrami:

```javascript
function greetPerson(name) {
    console.log("Witaj, " + name + "!");
}

// Wywołanie funkcji z argumentem
greetPerson("Jan");
```

#### Funkcje zwracające wartość:

```javascript
function add(a, b) {
    return a + b;
}

// Wywołanie funkcji i przechwycenie zwracanej wartości
let result = add(3, 5);
console.log(result); // Wyświetli: 8
```

#### Funkcje anonimowe:

Funkcje anonimowe to funkcje bez nazwy, które są przypisywane do zmiennej lub wykorzystywane jako argument w innej funkcji.

```javascript
let multiply = function(x, y) {
    return x * y;
};

// Wywołanie funkcji anonimowej
console.log(multiply(4, 6)); // Wyświetli: 24
```

#### Wyrażenia funkcyjne (Arrow Functions) - wprowadzone w ECMAScript 6:

```javascript
const square = (num) => {
    return num * num;
};

// Wywołanie funkcji
console.log(square(5)); // Wyświetli: 25
```

Funkcje w JavaScript są obiektami pierwszej klasy, co oznacza, że mogą być przypisywane do zmiennych, przekazywane jako argumenty do innych funkcji i zwracane z innych funkcji. Pozwalają one na organizację kodu, ponowne wykorzystanie, abstrakcję i wiele innych zaawansowanych technik programistycznych.

### Jak dodać javascript do strony?&#x20;

Istnieje kilka sposobów dodawania kodu JavaScript do strony internetowej. Oto kilka podstawowych metod:

#### 1. Tag `<script>` w sekcji `<head>` lub `<body>`:

Możesz umieścić kod JavaScript bezpośrednio wewnątrz tagu `<script>` w sekcji `<head>` lub `<body>` HTML.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Moja strona z JavaScriptem</title>
    <script>
        // Twój kod JavaScript
        function greet() {
            console.log("Witaj, świecie!");
        }
    </script>
</head>
<body>
    <!-- Treść strony -->
    <button onclick="greet()">Kliknij mnie</button>
</body>
</html>
```

#### 2. Zewnętrzny plik JavaScript:

Możesz również umieścić kod JavaScript w osobnym pliku `.js` i zaimportować go do strony za pomocą tagu `<script>`.

Plik `script.js`:

```javascript
// Twój kod JavaScript
function greet() {
    console.log("Witaj, świecie!");
}
```

HTML:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Moja strona z JavaScriptem</title>
    <script src="script.js"></script>
</head>
<body>
    <!-- Treść strony -->
    <button onclick="greet()">Kliknij mnie</button>
</body>
</html>
```

#### 3. Atrybut `defer` lub `async`:

Możesz użyć atrybutu `defer` lub `async` w tagu `<script>` w celu kontrolowania momentu ładowania i wykonania kodu JavaScript.

* `defer`: Ładuje skrypt w tle i wykonuje go po załadowaniu całej strony.
* `async`: Ładuje skrypt równolegle z przetwarzaniem strony i wykonuje go natychmiast po załadowaniu.

```html
<script src="script.js" defer></script>
```

```html
<script src="script.js" async></script>
```

Wybór sposobu zależy od potrzeb strony i oczekiwanego zachowania kodu JavaScript. Warto również pamiętać o umiejętności zarządzania zależnościami, organizacji kodu oraz jego optymalizacji dla wydajności strony.
