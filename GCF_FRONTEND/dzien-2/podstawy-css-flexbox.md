---
description: >-
  Zapoznanie się z flexboksem, żeby móc efektywnie układać elementy na stronie w
  pionie i w poziomie
coverY: 0
---

# 3 Podstawy CSS – flexbox

Flexbox to nowoczesny mechanizm w CSS, który ułatwia projektowanie elastycznych i responsywnych układów strony. Pozwala na łatwe zarządzanie rozmieszczeniem elementów w kontenerze, dostosowując je do różnych rozmiarów ekranu i dostarczając elastyczny sposób na zarządzanie przestrzenią wewnątrz kontenera.

Poniżej przedstawiam podstawowe pojęcia związane z flexbox:

#### Właściwość `display: flex`:

Aby uruchomić model flexbox na elemencie i uczynić go kontenerem elastycznym, używamy właściwości `display: flex` lub `display: inline-flex` (jeśli chcemy, aby element zachowywał się jak element inline).

```css
.container {
  display: flex;
}
```

#### Podstawowe Terminy:

1. **Flex Container (Kontener elastyczny):**
   * Element, który ma ustawioną właściwość `display: flex` lub `display: inline-flex`. Staje się kontenerem dla elementów potomnych, które zostaną ustawione w układzie flexbox.
2. **Flex Items (Elementy elastyczne):**
   * Elementy potomne kontenera flexbox, które zostaną ustawione w układzie flexbox.
3. **Main Axis (Główna oś) i Cross Axis (Poprzeczna oś):**
   * W flexboxie istnieją dwie osie - główna (main axis) i poprzeczna (cross axis). Główna oś to kierunek, w którym elementy są ustawiane, a poprzeczna oś jest prostopadła do głównej osi.

#### Podstawowe Właściwości Flexbox:

1.  **`flex-direction`:**

    * Określa kierunek, w jakim elementy są ustawiane na głównej osi. Może być ustawione na `row`, `row-reverse`, `column`, `column-reverse`.

    ```css
    .container {
      flex-direction: row; /* Domyślnie od lewej do prawej */
    }
    ```
2.  **`justify-content`:**

    * Określa, jak elementy są rozmieszczane wzdłuż głównej osi. Może przyjąć wartości takie jak `flex-start`, `flex-end`, `center`, `space-between`, `space-around`.

    ```css
    .container {
      justify-content: space-between; /* Rozkładane równomiernie z odstępem między nimi */
    }
    ```
3.  **`align-items`:**

    * Określa, jak elementy są rozmieszczane wzdłuż poprzecznej osi. Może przyjąć wartości takie jak `flex-start`, `flex-end`, `center`, `baseline`, `stretch`.

    ```css
    .container {
      align-items: center; /* Wyśrodkowane na osi poprzecznej */
    }
    ```
4.  **`flex`:**

    * Określa, jak elementy elastyczne mają rozszerzać się w stosunku do siebie. Składa się z trzech wartości: `flex-grow`, `flex-shrink`, i `flex-basis`.

    ```css
    .flex-item {
      flex: 1 0 200px; /* Rozszerza się, nie kurczy się, bazowa szerokość 200px */
    }
    ```
5.  **`align-self`:**

    * Pozwala na nadpisanie właściwości `align-items` dla konkretnego elementu elastycznego.

    ```css
    .flex-item {
      align-self: flex-end; /* Wyjustowane do końca na osi poprzecznej */
    }
    ```

Flexbox dostarcza wiele innych właściwości i wartości, które pozwalają na dokładne dostosowanie układu elastycznego do potrzeb projektu. Jest to potężne narzędzie do responsywnego projektowania stron internetowych.

<figure><img src="../.gitbook/assets/css-flexbox-poster.png" alt=""><figcaption></figcaption></figure>

​​📗**Materiały dodatkowe:**

{% embed url="https://css-tricks.com/snippets/css/a-guide-to-flexbox/" %}

{% embed url="https://flexboxfroggy.com/#pl" %}

{% embed url="https://flexboxzombies.com/p/flexbox-zombies" %}
