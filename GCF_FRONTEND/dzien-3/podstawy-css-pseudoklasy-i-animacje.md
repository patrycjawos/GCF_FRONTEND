---
coverY: 0
---

# 2️ Podstawy CSS – pseudoklasy i animacje

### Pseudoklasy

Pseudoklasy w CSS to specjalne selektory, które pozwalają aplikować styl do elementów w określonych stanach lub relacjach z dokumentem HTML. Te stany mogą być interaktywne (jak `:hover` po najechaniu myszką) lub bazować na strukturze dokumentu (jak `:first-child` dla pierwszego dziecka elementu).

Oto kilka przykładów pseudoklas:

1. `:hover`: Styl aplikowany, gdy kursor znajduje się nad elementem. Na przykład, zmiana koloru tekstu po najechaniu myszką na link.

```css
cssCopy codea:hover {
  color: red;
}
```

2. `:first-child`: Styl aplikowany do pierwszego dziecka elementu. Można użyć tego, aby zmienić styl pierwszego elementu wewnątrz kontenera.

```css
cssCopy codeli:first-child {
  font-weight: bold;
}
```

3. `:nth-child(n)`: Wybiera elementy na podstawie ich numeru w kontenerze. Na przykład, można wybrać co drugi element lub konkretne numery.

```css
cssCopy codetr:nth-child(odd) {
  background-color: #f2f2f2;
}
```

4. `:focus`: Styl aplikowany, gdy element ma focus. Jest używane często w formularzach, aby zaznaczyć aktywny element.

```css
cssCopy codeinput:focus {
  border: 1px solid blue;
}
```

Pseudoklasy mogą być używane w wielu kontekstach do dostosowywania wyglądu i interakcji elementów w zależności od ich stanów lub ich relacji z innymi elementami w strukturze dokumentu. Są one użyteczne w celu tworzenia bardziej interaktywnych i dynamicznych interfejsów użytkownika.

### Animacje w CSS – transition

Transition to właściwość w CSS, która umożliwia płynne przejścia między różnymi stanami elementów, np. zmiany koloru, rozmiaru, położenia itp. Wprowadza płynne przejścia między wartościami właściwości CSS, gdy te wartości ulegają zmianie.

Aby zdefiniować przejście, używa się właściwości `transition` wraz z określeniem, które własności CSS mają być animowane, czasem trwania animacji oraz ewentualnym opóźnieniem rozpoczęcia animacji.

Ogólna składnia właściwości `transition` wygląda tak:

```css
cssCopy codeselector {
  transition: property duration timing-function delay;
}
```

* `property`: Określa, którą właściwość CSS chcemy animować (np. `color`, `width`, `height`).
* `duration`: Określa czas trwania animacji w sekundach lub milisekundach.
* `timing-function`: Opcjonalny parametr, który kontroluje sposób, w jaki przejście zmienia się w czasie (np. `ease`, `linear`, `ease-in-out`).
* `delay`: Opcjonalny parametr, który określa opóźnienie przed rozpoczęciem animacji.

Przykład użycia transition:

```css
cssCopy codebutton {
  background-color: #3498db;
  color: #fff;
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: #2980b9;
}
```

W tym przykładzie, gdy kursor najedzie na przycisk (`:hover`), zmiana koloru tła zostanie płynnie wykonana w ciągu 0.3 sekundy (`transition: background-color 0.3s ease;`).

`Transition` jest potężnym narzędziem do dodawania efektów interakcji do stron internetowych, zapewniając płynne zmiany między stanami elementów i poprawiając doświadczenie użytkownika. Możesz użyć tego mechanizmu, aby nadać swojej stronie dynamiczność i atrakcyjność wizualną.

#### Playground:: [https://developer.mozilla.org/en-US/docs/Web/CSS/transition](https://developer.mozilla.org/en-US/docs/Web/CSS/transition)

###

### Animacje w CSS – transform

Właściwość `transform` w CSS umożliwia wykonywanie różnych przekształceń (np. translacji, skalowania, obracania, pochylania) elementów HTML bez zmieniania ich rzeczywistego układu w dokumencie. Pozwala na manipulowanie wyglądem i pozycją elementów w sposób graficzny.

`Transform` pozwala na stosowanie różnych rodzajów transformacji za pomocą jednej właściwości, poprzez użycie różnych funkcji transformacji jako jej wartości.

Oto kilka rodzajów transformacji, jakie można zastosować za pomocą właściwości `transform`:

1. **Translacja (`translate`):** Przesuwanie elementu w poziomie i pionie.

```css
cssCopy code.element {
  transform: translate(50px, 20px);
}
```

2. **Skalowanie (`scale`):** Zmiana rozmiaru elementu wzdłuż osi X i Y.

```css
cssCopy code.element {
  transform: scale(1.5);
}
```

3. **Obracanie (`rotate`):** Obracanie elementu o określony kąt.

```css
cssCopy code.element {
  transform: rotate(45deg);
}
```

4. **Pochylenie (`skew`):** Pochylanie elementu wzdłuż osi X i Y.

```css
cssCopy code.element {
  transform: skew(20deg, 10deg);
}
```

5. **Kombinacja transformacji:** Można łączyć różne transformacje w jednej deklaracji.

```css
cssCopy code.element {
  transform: translate(50px, 50px) rotate(45deg) scale(1.2);
}
```

Wartości funkcji transformacji mogą być wyrażane w pikselach (`px`), procentach (`%`), stopniach (`deg`) lub innych jednostkach długości, zależnie od rodzaju transformacji.

Właściwość `transform` jest potężnym narzędziem do manipulowania wyglądem elementów na stronie internetowej. Pozwala na płynne zmiany wizualne i interakcje, często wykorzystywane przy tworzeniu animacji, efektów przejść oraz interaktywnych elementów na stronie.

#### Playground: [https://developer.mozilla.org/en-US/docs/Web/CSS/transform](https://developer.mozilla.org/en-US/docs/Web/CSS/transform)

<br>
