#Website: https://leonard-roepcke.github.io/it-Fragen/
# it-Fragen
HTML5 Apps zu IT-Fragen




temp
1. **Warum braucht man die indexGueltig-Funktion überhaupt?**
   - *Antwort: Um vor Zugriffen zu prüfen, ob ein Index existiert und Abstürze zu vermeiden.*

2. **Welche drei Fälle kann indexGueltig zurückgeben und wann?**
   - *Antwort: FALSCH bei negativem Index, FALSCH bei Index > Listenlänge, WAHR bei gültigem Index.*

3. **Was wäre das Problem, wenn man die Prüfung `pIndex < 0` weglassen würde?**
   - *Antwort: Man würde versuchen, auf negative Positionen zuzugreifen, was immer ungültig ist und zu Fehlern führt.*

4. **Wie würde sich der Algorithmus ändern, wenn wir doppelt verkettete Listen hätten?**
    - *Antwort: Wir müssten auch den Rückwärtszeiger (vorheriger) des neuen Knotens und seines Nachfolgers setzen.*

5. **Was passiert bei `indexGueltig(0)` in einer nicht-leeren Liste?**
   - *Antwort: Die Schleife wird übersprungen (i < 0 ist falsch) und direkt WAHR zurückgegeben - Index 0 ist immer gültig, wenn Liste nicht leer.*


6. **Warum navigieren wir bei elementEinfuegen nur bis Position pos-1 und nicht bis pos?**
   - *Antwort: Weil wir den Vorgängerknoten brauchen, dessen Zeiger wir ändern müssen - nicht den Knoten an der Einfügeposition selbst.*

7. **Wie viele Zeiger-Änderungen sind beim Einfügen in der Listenmitte nötig?**
   - *Antwort: Genau zwei: 1) Neuer Knoten zeigt auf Nachfolger, 2) Vorgänger zeigt auf neuen Knoten.*

8. **Was ist der Unterschied beim Einfügen an Position 0 gegenüber anderen Positionen?**
   - *Antwort: Bei Position 0 muss der Start-Zeiger der gesamten Liste angepasst werden, nicht nur ein Knotenzeiger.*

9. **Warum ist das Einfügen in verketteten Listen oft effizienter als in Arrays?**
   - *Antwort: Weil bei Arrays Elemente verschoben werden müssen (O(n)), während bei Listen nur Zeiger geändert werden (O(1) nach Navigation).*

10. **Wie können indexGueltig und elementEinfuegen zusammenarbeiten?**
    - *Antwort: indexGueltig kann vor elementEinfuegen aufgerufen werden, um zu prüfen, ob die Einfügeposition gültig ist (oder mindestens pos-1 existiert).*