---
description: >-
  Dodanie stylów CSS do poszczególnych sekcji na stronie ze szczególnym
  naciskiem na wyświetlanie elementów (display) i box-model
coverY: 0
---

# 2⃣ Podstawy CSS 3 – display i box-model

### Normalize.css&#x20;

Przeglądarki mają swoje wbudowane style CSS, które różnią się w zależności od przeglądarki. Żeby to trochę ujednolicić, można dodać kolejny arkusz stylów: normalize.css.&#x20;

{% embed url="https://necolas.github.io/normalize.css/" %}

### Display

Właściwość `display` w CSS służy do kontrolowania sposobu, w jaki element HTML jest renderowany na stronie. Określa, jak element ma być wyświetlany w przeglądarce. Poniżej przedstawiam kilka najważniejszych wartości, jakie można przypisać właściwości `display`:

1.  **`block`:**

    * Element jest renderowany jako blokowy, zajmujący pełną dostępną szerokość na stronie. Elementy blokowe zawsze zaczynają się od nowej linii i rozciągają się na całą szerokość swojego kontenera.

    ```css
    div {
      display: block;
    }
    ```
2.  **`inline`:**

    * Element jest renderowany jako element wiersza, który nie zaczyna od nowej linii i zajmuje tyle szerokości, ile to konieczne, aby pomieścić jego zawartość.

    ```css
    span {
      display: inline;
    }
    ```
3.  **`inline-block`:**

    * Element jest renderowany jako element wiersza, ale zachowuje się jak blokowy pod względem modelu pudełkowego, co oznacza, że można mu przypisać szerokość i wysokość.

    ```css
    img {
      display: inline-block;
    }
    ```
4.  **`none`:**

    * Element jest ukryty i nie zajmuje miejsca na stronie. Jest to często używane, aby dynamicznie ukryć i pokazać elementy w zależności od warunków.

    ```css
    #ukryty-element {
      display: none;
    }
    ```
5.  **`flex`:**

    * Element jest renderowany jako elastyczny kontener, który może dostosowywać swoje elementy potomne zarówno wzdłuż osi głównej (wiersz) jak i poprzecznej (kolumna).

    ```css
    .flex-container {
      display: flex;
    }
    ```
6.  **`grid`:**

    * Element jest renderowany jako kontener siatki, który ułatwia rozmieszczanie elementów w dwuwymiarowym układzie.

    ```css
    .grid-container {
      display: grid;
    }
    ```
7.  **`table`:**

    * Element zachowuje się jak element tabeli, co oznacza, że może mieć elementy potomne takie jak `table-row`, `table-cell`, itp.

    ```css
    .table {
      display: table;
    }
    ```



### Box model

Model pudełkowy (ang. box model) w CSS to fundamentalna koncepcja, która opisuje sposób renderowania i organizowania elementów na stronie internetowej. Każdy element HTML jest traktowany jako prostokąt, a model pudełkowy definiuje strukturę tego prostokąta. Model pudełkowy składa się z kilku składowych, które określają, jak element będzie wyglądał i jak będzie zachowywał się w kontekście innych elementów na stronie.

Główne składowe modelu pudełkowego to:

1. **Content (Zawartość):**
   * To wnętrze prostokąta, w którym znajduje się faktyczna treść elementu, tak jak tekst, obraz czy inne elementy potomne.
2. **Padding (Margines wewnętrzny):**
   * To obszar między zawartością a ramką (borderem). Padding definiuje przestrzeń wewnątrz elementu, oddzielającą zawartość od obramowania.
3. **Border (Obramowanie):**
   * Obramowanie określa widoczny kontur elementu. Jest to linia otaczająca padding, która może mieć różne style, grubości i kolory.
4. **Margin (Margines zewnętrzny):**
   * Margines zewnętrzny to obszar między obramowaniem a sąsiednimi elementami. Margines kontroluje odstęp między aktualnym elementem a sąsiadującymi elementami na stronie.

Poniżej przedstawiam przykład, jak wygląda model pudełkowy w formie schematu:

{% embed url="https://codepen.io/Sneha_Raut/pen/zYaaOgv" %}

W praktyce można dostosowywać każdy z tych składników, korzystając z właściwości CSS. Na przykład, można zmieniać szerokość i wysokość elementu poprzez manipulację contentem, paddingiem, borderem i marginem.

Przykładowa deklaracja CSS dla prostego diva z modelem pudełkowym może wyglądać tak:

```css
div {
  width: 200px;          /* Szerokość contentu */
  height: 100px;         /* Wysokość contentu */
  padding: 20px;         /* Padding wewnątrz */
  border: 2px solid #000; /* Grubość, styl i kolor obramowania */
  margin: 10px;          /* Margines na zewnątrz */
}
```

Model pudełkowy jest kluczowym aspektem projektowania stron internetowych, ponieważ pozwala precyzyjnie kontrolować układ elementów na stronie.

### Box-sizing

Właściwość `box-sizing` w CSS jest używana do kontrolowania modelu pudełkowego (box model) elementów. Jednym z najczęstszych zastosowań tej właściwości jest zmiana sposobu, w jaki szerokość i wysokość elementów są obliczane, uwzględniając lub ignorując padding i border.

Istnieją dwie główne wartości właściwości `box-sizing`:

1.  **`content-box` (domyślna):**

    * Jest to standardowa wartość. Szerokość i wysokość elementu obejmują tylko zawartość (content), bez uwzględniania paddingu, obramowania (border) i marginesu.

    ```css
    .element {
      box-sizing: content-box;
    }
    ```
2.  **`border-box`:**

    * Wartość `border-box` zmienia sposób obliczania szerokości i wysokości elementu. Teraz szerokość elementu obejmuje zawartość, padding i obramowanie, ale nie margines.

    ```css
    .element {
      box-sizing: border-box;
    }
    ```

Przykład z `border-box` może być szczególnie użyteczny w sytuacjach, w których chcemy precyzyjnie kontrolować szerokość elementu, a jednocześnie uwzględniać padding i obramowanie. Na przykład:

```css
/* Domyślny box-sizing: content-box */
.element {
  width: 200px;       /* Szerokość contentu */
  padding: 20px;      /* Padding wewnątrz */
  border: 2px solid;  /* Obramowanie */
  /* Całkowita szerokość elementu to 244px (200 + 2*20 + 2*2) */
}

/* Ustawienie box-sizing: border-box */
.element {
  box-sizing: border-box;
  width: 200px;       /* Całkowita szerokość elementu to teraz dokładnie 200px */
  padding: 20px;      /* Padding wewnątrz */
  border: 2px solid;  /* Obramowanie */
}
```

Ustawienie `box-sizing: border-box` może ułatwić pracę z layoutem, szczególnie gdy projektujesz elastyczne układy i chcesz uniknąć niespodziewanych zmian w szerokości elementów wynikających z dodania paddingu czy obramowania.

{% embed url="https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing" %}

### Background-image

Właściwość `background-image` w CSS służy do określania obrazu tła dla elementu HTML. Pozwala dodawać grafikę, obraz lub wzór jako tło dla danego elementu. Poniżej znajdziesz podstawowe informacje na temat tej właściwości:

#### Składnia:

```css
selector {
  background-image: url('ścieżka/do/pliku.jpg');
}
```

#### Właściwości powiązane z `background-image`:

1.  **`background-repeat`:**

    * Określa, czy obraz tła powinien być powtarzany (domyślnie) wzdłuż i wszerz, tylko wzdłuż, tylko wszerz lub nie powinien być powtarzany w ogóle.

    ```css
    selector {
      background-image: url('ścieżka/do/pliku.jpg');
      background-repeat: no-repeat;
    }
    ```
2.  **`background-size`:**

    * Kontroluje wielkość obrazu tła. Może być ustawione na wartości takie jak `cover` (aby całe tło było pokryte), `contain` (aby całe tło było widoczne), lub konkretne wartości w pikselach lub procentach.

    ```css
    selector {
      background-image: url('ścieżka/do/pliku.jpg');
      background-size: cover;
    }
    ```
3.  **`background-position`:**

    * Określa położenie obrazu tła wewnątrz elementu. Możesz używać wartości procentowych, pikseli lub słów kluczowych, takich jak `center`, `left`, `right`, `top`, `bottom`.

    ```css
    selector {
      background-image: url('ścieżka/do/pliku.jpg');
      background-position: center;
    }
    ```
4.  **`background-attachment`:**

    * Określa, czy obraz tła powinien być przewijany wraz ze stroną (`scroll`) czy być przyklejony do widoku (`fixed`).

    ```css
    selector {
      background-image: url('ścieżka/do/pliku.jpg');
      background-attachment: fixed;
    }
    ```

#### Przykładowe użycie:

```css
body {
  background-image: url('background.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
}
```

W powyższym przykładzie ustawiamy obraz o nazwie 'background.jpg' jako tło dla całego body. Nie powtarzamy go (`no-repeat`), dopasowujemy do szerokości i wysokości ekranu (`cover`), ustawiamy w centrum (`center`) i przyklejamy do widoku (`fixed`).

{% embed url="https://developer.mozilla.org/en-US/docs/Web/CSS/background-position" %}

{% embed url="https://developer.mozilla.org/en-US/docs/Web/CSS/background-size" %}



### Background-color

Właściwość `background-color` w CSS służy do określania koloru tła dla elementu HTML. Pozwala ustawić jednolity kolor tła, który może być widoczny, gdy nie ma ustawionego obrazu tła lub gdy obraz tła jest trasowany przez przezroczyste obszary.

#### Składnia:

```css
selector {
  background-color: nazwa_koloru;
}
```

#### Właściwości powiązane z `background-color`:

1.  **Kolor w formie nazwy:**

    ```css
    selector {
      background-color: red;
    }
    ```
2.  **Kolor w formie wartości heksadecymalnej:**

    ```css
    selector {
      background-color: #ff0000;
    }
    ```
3.  **Kolor w formie wartości RGB:**

    ```css
    selector {
      background-color: rgb(255, 0, 0);
    }
    ```
4.  **Przezroczystość:**

    * Możesz również użyć funkcji `rgba` lub `hsla`, aby określić kolor z przejrzystością (alpha), co pozwala na widoczność elementów znajdujących się pod elementem z kolorowym tłem.

    ```css
    selector {
      background-color: rgba(255, 0, 0, 0.5); /* Przezroczystość ustawiona na 0.5 */
    }
    ```

#### Przykłady użycia:

1.  **Ustawienie koloru tła na czerwony:**

    ```css
    body {
      background-color: red;
    }
    ```
2.  **Ustawienie koloru tła na niebieski za pomocą wartości heksadecymalnej:**

    ```css
    .container {
      background-color: #0000ff;
    }
    ```
3.  **Ustawienie koloru tła na zielony za pomocą wartości RGB:**

    ```css
    .header {
      background-color: rgb(0, 255, 0);
    }
    ```
4.  **Ustawienie koloru tła na żółty z przezroczystością:**

    ```css
    .overlay {
      background-color: rgba(255, 255, 0, 0.7);
    }
    ```

Właściwość `background-color` jest podstawowym narzędziem do kontrolowania wyglądu tła elementu wizualnego na stronie internetowej. Możesz dostosować kolor, a także dodatkowe właściwości tła, takie jak obraz tła czy właściwości związane z powtarzaniem i pozycjonowaniem.



### Dziedziczenie w CSS&#x20;

Dziedziczenie w CSS to mechanizm, który pozwala na przekazywanie pewnych stylów z jednego elementu na potomne elementy w strukturze drzewa dokumentu. Dziedziczenie umożliwia bardziej skondensowane i spójne arkusze stylów, ponieważ nie trzeba dla każdego elementu ponownie deklarować tych samych stylów, które są dziedziczone.

W kontekście CSS, nie wszystkie właściwości są dziedziczone domyślnie. Niektóre właściwości są dziedziczone, co oznacza, że wartość danej właściwości przekazywana jest z elementu nadrzędnego na elementy podrzędne. Inne właściwości nie są dziedziczone i muszą być jawne dla każdego elementu potomnego.

Przykłady właściwości dziedziczonych to:

1. **Kolor tekstu (`color`):**
   * Dziedziczy się z elementu nadrzędnego na elementy potomne.
2. **Czcionka (`font-family`, `font-size`, `font-weight` itp.):**
   * Wiele właściwości związanych z czcionką jest dziedziczonych.
3. **Styl tekstu (`font-style`):**
   * Styl tekstu, tak jak "italic" czy "oblique", jest dziedziczony.
4. **Wielkość (`line-height`):**
   * Wysokość linii jest dziedziczona.
5. **Tekstowymyjustowanie (`text-align`):**
   * Właściwość określająca justowanie tekstu dziedziczy się.

Przykłady właściwości, które nie są dziedziczone, to:

1. **Wysokość (`height`), szerokość (`width`):**
   * Te właściwości nie są dziedziczone. Każdy element musi określić swoje własne wymiary.
2. **Wizualne efekty (`background`, `border`, `margin`, `padding`):**
   * Wizualne efekty, takie jak tło, obramowanie, marginesy i paddingi, zazwyczaj nie są dziedziczone. Każdy element musi określić te wartości indywidualnie.
3. **Właściwości związane z pozycjonowaniem (`position`, `top`, `left` itp.):**
   * Właściwości związane z pozycjonowaniem elementu również nie są dziedziczone.

Aby sprawdzić, czy dana właściwość jest dziedziczona, warto zajrzeć do dokumentacji CSS dla konkretnej właściwości. Jeśli jest dziedziczona, wartość zastosowana do elementu nadrzędnego będzie dziedziczona przez elementy potomne, chyba że zostanie nadpisana przez konkretne deklaracje stylów dla tych elementów potomnych.



**Podsumowanie**

* ?
* ?

​​📗**Materiały dodatkowe:**​
