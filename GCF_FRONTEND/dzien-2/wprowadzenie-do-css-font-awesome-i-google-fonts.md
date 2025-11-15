---
description: >-
  Przedstawienie, czym jest CSS, jaka jest jego składnia i poznanie podstaw
  dotyczących edycji tekstu, kolorów. Dodawanie klas i identyfikatorów w pliku
  HTML. Wykorzystanie selektorów do stylowania.
coverY: 0
---

# 1️ Wprowadzenie do CSS, Font Awesome i Google Fonts

**CSS, czyli Cascading Style Sheets,** to język stylów używany do opisywania wyglądu i formatowania dokumentów HTML (lub XML). CSS umożliwia separację struktury dokumentu od jego prezentacji, co pozwala na lepszą kontrolę nad wyglądem strony internetowej.

Termin "Cascading" w CSS oznacza, że style mogą być dziedziczone lub nadpisywane z różnych źródeł, tworząc kaskadę zasad stylów. Istnieje hierarchia priorytetów w dziedziczeniu i nadpisywaniu stylów, co pozwala na elastyczne zarządzanie wyglądem strony. Priorytety te są określane przez trzy główne źródła stylów:

1. **Autor (Autor Styles):** To style określone przez autora strony internetowej. Są to zazwyczaj style definiowane bezpośrednio w arkuszu stylów CSS.
2. **Użytkownik (User Styles):** Style, które użytkownik może zastosować do dostosowania wyglądu stron według swoich preferencji. Można to osiągnąć poprzez przeglądarkę internetową lub inne narzędzia, które pozwalają na dostosowanie stylów stron internetowych.
3. **Agent użytkownika (User Agent Styles):** Są to domyślne style określone przez przeglądarkę internetową. Jeśli autor strony nie określi pewnych stylów, przeglądarka użyje swoich domyślnych ustawień.

Ponadto, istnieje specyficzny porządek, w jakim style są aplikowane w kaskadzie. Generalnie rzecz biorąc, bardziej szczegółowe i specyficzne style mają wyższy priorytet niż ogólne style. Na przykład, style zdefiniowane bezpośrednio dla konkretnego elementu HTML mają większy priorytet niż ogólne style dla wszystkich elementów tego typu.

Przykładowe zastosowanie CSS w HTML może wyglądać tak:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Strona z CSS</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            color: #333;
        }

        h1 {
            color: #0077cc;
        }

        .container {
            width: 80%;
            margin: 0 auto;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>Witaj na mojej stronie!</h1>
        <p>To jest przykładowy tekst na stronie z zastosowanymi stylami CSS.</p>
    </div>

</body>
</html>

```

W tym przykładzie, style są definiowane bezpośrednio w sekcji `<style>` w nagłówku HTML, ale często są również przechowywane w zewnętrznych plikach CSS, co pozwala na lepszą organizację i zarządzanie nimi.



### Stylowanie tekstu

Stylowanie fontu w CSS można osiągnąć za pomocą różnych właściwości i wartości. Oto kilka popularnych właściwości CSS używanych do stylizacji fontu:

1.  **font-family:** Określa rodzinę fontów, które mają być używane na stronie. Jeśli pierwszy wybór nie jest dostępny, przeglądarka spróbuje użyć kolejnych w kolejności.

    ```css
    body {
        font-family: "Arial", sans-serif;
    }
    ```
2.  **font-size:** Ustala wielkość fontu. Można używać różnych jednostek, takich jak piksele, em, procenty itp.

    ```css
    h1 {
        font-size: 24px;
    }
    ```
3.  **font-weight:** Określa grubość fontu. Może przyjmować wartości, takie jak `normal`, `bold`, `bolder`, `lighter`, lub wartości numeryczne.

    ```css
    p {
        font-weight: bold;
    }
    ```
4.  **font-style:** Określa styl fontu, takie jak `normal`, `italic` lub `oblique`.

    ```css
    em {
        font-style: italic;
    }
    ```
5.  **text-transform:** Zmienia wielkość liter w tekście. Może przyjmować wartości, takie jak `uppercase`, `lowercase` lub `capitalize`.

    ```css
    .uppercase-text {
        text-transform: uppercase;
    }
    ```
6.  **color:** Określa kolor tekstu.

    ```css
    h2 {
        color: #3366cc;
    }
    ```
7.  **line-height:** Określa odstęp między wierszami tekstu.

    ```css
    p {
        line-height: 1.5;
    }
    ```
8.  **letter-spacing:** Określa odstęp między literami.

    ```css
    .spaced-text {
        letter-spacing: 2px;
    }
    ```
9.  **text-align:** Określa justyfikację tekstu.

    ```css
    .centered-text {
        text-align: center;
    }
    ```
10. **text-decoration:** Określa dekorację tekstu, taką jak podkreślenie.

    ```css
    a {
        text-decoration: none;
    }
    ```

Te właściwości mogą być stosowane do różnych selektorów, takich jak elementy HTML, klasy czy identyfikatory, aby dostosować styl fontu do konkretnych elementów na stronie. Warto eksperymentować z różnymi wartościami, aby uzyskać pożądany efekt stylizacyjny.

### Kolory

W CSS można określać kolory na różne sposoby. Oto kilka popularnych sposobów definiowania kolorów w CSS:

1.  **Nazwy Kolorów:**

    ```css
    body {
        color: red;
        background-color: lightblue;
    }
    ```

    W CSS istnieje kilka nazwanych kolorów, takich jak `red`, `blue`, `green`, itp. Pełna lista nazwanych kolorów jest dostępna w specyfikacji CSS.
2.  **Kody Kolorów Hex:**

    ```css
    h1 {
        color: #ff0000; /* czerwony */
        background-color: #00ff00; /* zielony */
    }
    ```

    Kody kolorów w formacie szesnastkowym (#RRGGBB) pozwalają na precyzyjne określenie koloru za pomocą trzech składowych: czerwonej (RR), zielonej (GG) i niebieskiej (BB).
3.  **Kody Kolorów RGB:**

    ```css
    p {
        color: rgb(255, 0, 255); /* fioletowy */
        background-color: rgb(0, 128, 255); /* jasnoniebieski */
    }
    ```

    Kody kolorów RGB (Red, Green, Blue) pozwalają na określenie koloru poprzez wartości intensywności dla każdej z trzech składowych.
4.  **Kody Kolorów RGBA:**

    ```css
    div {
        background-color: rgba(255, 0, 0, 0.3); /* czerwony z przezroczystością 30% */
    }
    ```

    Kody kolorów RGBA są podobne do RGB, ale zawierają dodatkowy parametr dla przezroczystości (Alpha). Wartość alfa może mieć zakres od 0 (całkowicie przezroczysty) do 1 (całkowicie nieprzezroczysty).
5.  **Kody Kolorów HSL:**

    ```css
    span {
        color: hsl(120, 100%, 50%); /* zielony w przestrzeni HSL */
    }
    ```

    Kody kolorów HSL (Hue, Saturation, Lightness) pozwalają na określenie koloru za pomocą barwy, nasycenia i jasności.
6.  **Kody Kolorów HSLA:**

    ```css
    a {
        color: hsla(240, 100%, 50%, 0.5); /* niebieski z przezroczystością 50% */
    }
    ```

    Kody kolorów HSLA są podobne do HSL, ale zawierają również parametr alfa dla przezroczystości.

Dobrze jest wybierać sposób określania kolorów w zależności od potrzeb i preferencji, a także biorąc pod uwagę dostępność i czytelność kolorów na różnych urządzeniach.

### Google Fonts

[https://fonts.google.com/](wprowadzenie-do-css-font-awesome-i-google-fonts.md#google-fonts)

### Ikonki - SVG

\
**SVG (Scalable Vector Graphics)** -  to format plików graficznych, który jest używany do reprezentowania dwuwymiarowej grafiki wektorowej w sposób skalowalny, czyli bez utraty jakości przy zmianie rozmiaru (w porównaniu do PNG np). SVG jest popularny w tworzeniu ikon, grafik, animacji i innych elementów interfejsu użytkownika na stronach internetowych.\
\
**Baza \~ 1500 darmowych ikonek svg**&#x20;

{% embed url="https://iconoir.com/" %}



**Podsumowanie**

* ?
* ?

​​📗**Materiały dodatkowe:**&#x200B;
