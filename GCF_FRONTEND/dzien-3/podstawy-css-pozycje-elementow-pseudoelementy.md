---
coverY: 0
---

# 1️ Podstawy CSS – pozycje elementów, pseudoelementy

### Position

Właściwość `position` w CSS kontroluje sposób, w jaki element jest pozycjonowany w obrębie strony internetowej. Możesz użyć jej do manipulowania położeniem elementów na stronie.

Istnieją cztery główne wartości właściwości `position`:

1. `static`: Jest to wartość domyślna. Elementy z pozycją `static` są umieszczane w zwykłym układzie strony. Nie są one przesuwane na podstawie żadnych innych właściwości pozycjonowania (takich jak `top`, `bottom`, `left`, `right`). Te właściwości nie mają wpływu na elementy z pozycją `static`.
2. `relative`: Pozycjonuje element względem jego pierwotnego położenia. Możesz użyć właściwości `top`, `bottom`, `left`, `right`, aby przesunąć element względem jego pozycji wyjściowej, ale element ten nadal zajmuje swoje pierwotne miejsce w przepływie dokumentu.
3. `absolute`: Pozycjonuje element względem jego najbliższego rodzica, który ma ustawioną pozycję inną niż `static`. Jeśli żaden rodzic nie ma ustawionej pozycji innej niż `static`, element z pozycją `absolute` odnosi się do ciała dokumentu (`<body>`). Elementy z ustawioną pozycją `absolute` są usuwane z naturalnego przepływu dokumentu, co oznacza, że inne elementy mogą zajmować ich miejsce.
4. `fixed`: Pozycjonuje element względem okna przeglądarki. Element z pozycją `fixed` będzie trzymał się okna przeglądarki nawet wtedy, gdy przewijasz stronę. To przydatne do tworzenia elementów, które powinny być zawsze widoczne na ekranie, na przykład paska nawigacyjnego.

Warto pamiętać, że używanie właściwości `position` często łączy się z innymi właściwościami, takimi jak `top`, `bottom`, `left`, `right`, aby precyzyjnie kontrolować położenie elementu na stronie. Praktyczne eksperymentowanie i testowanie różnych kombinacji pomaga zrozumieć, jak `position` wpływa na układ strony.

Przykład:&#x20;

{% embed url="https://codepen.io/cheryllium/pen/GrBobz?editors=1100" %}

### Pseudoelementy&#x20;

Pseudoelementy w CSS to specjalne selektory, które pozwalają tworzyć stylizowane części elementów, które nie istnieją jako rzeczywiste elementy HTML. Są one używane do dodawania dekoracji, stylów lub zawartości do elementów na stronie, które nie istnieją w strukturze DOM.

Pseudoelementy rozpoczynają się dwukropkiem `::` i są dodawane do selektora, aby wybrać określoną część elementu. Dwa z najczęściej używanych pseudoelementów to:

1. `::before`: Pozwala dodać zawartość przed zawartością wybranego elementu. Można użyć tego pseudoelementu, aby wstawić dekoracyjne elementy, ikony, lub dodatkowy tekst przed wybranym elementem.

```css
cssCopy code.element::before {
  content: "Dodatkowy tekst ";
  font-weight: bold;
}
```

2. `::after`: Pozwala dodać zawartość po zawartości wybranego elementu. Można użyć tego pseudoelementu, aby wstawić dekoracyjne elementy lub treść za wybranym elementem.

```css
cssCopy code.element::after {
  content: " - Koniec";
  font-style: italic;
}
```

Pseudoelementy mogą być stylizowane za pomocą właściwości CSS takich jak `content`, `display`, `position`, `color`, `font`, itp. Są one przydatne do dodawania ozdobników, ikon, czy nawet funkcjonalności wizualnych do elementów strony bez konieczności dodawania dodatkowych elementów do struktury HTML.

### Z-index

Właściwość `z-index` w CSS kontroluje warstwy układu elementów, pozwalając określić, który element powinien być wyżej w stosunku do innych, jeśli nakładają się na siebie.

Działanie `z-index` ma sens tylko wtedy, gdy elementy mają ustawioną pozycję inną niż `static`. Elementy z pozycją `static` są ustawione w standardowym przepływie dokumentu i `z-index` na nie nie ma wpływu.

Główne punkty dotyczące `z-index`:

1. **Wyższe wartości `z-index` umieszczają elementy na wierzchu:** Im większa wartość `z-index`, tym element jest wyżej na stosie warstw. Elementy o wyższych wartościach `z-index` są renderowane na wierzchu innych elementów z niższymi wartościami `z-index`.
2. **Elementy potomne dziedziczą `z-index` od swoich rodziców:** Dziecko zwykle nie może wyjść poza warstwę z-index swojego rodzica. Jednakże, elementy potomne mogą mieć wyższe `z-index` w stosunku do innych elementów w tej samej warstwie z-index.
3. **Kontekst warstwy z-index:** Elementy z większym `z-index` są rysowane powyżej elementów z niższym `z-index`. Jednakże, jeśli elementy znajdują się w różnych kontekstach warstw, może to wpłynąć na sposób, w jaki zachowują się wartości `z-index`. Na przykład, elementy w ramach kontenerów z ustawionym `z-index` będą porównywane tylko w obrębie tych kontenerów, a nie globalnie w stosunku do wszystkich elementów na stronie.
4. **Zastosowanie do pozycji `absolute`, `fixed`, `relative`:** Wartość `z-index` działa głównie w kontekście elementów, które mają ustawioną pozycję `absolute`, `fixed` lub `relative`. Elementy te są usuwane z normalnego przepływu dokumentu, więc `z-index` pomaga kontrolować ich warstwowość na stronie.

Pamiętaj, że `z-index` jest często używane w połączeniu z innymi właściwościami pozycjonowania (takimi jak `position`) oraz może być używane do kontrolowania, które elementy są renderowane na wierzchu w przypadku nakładania się na siebie.
