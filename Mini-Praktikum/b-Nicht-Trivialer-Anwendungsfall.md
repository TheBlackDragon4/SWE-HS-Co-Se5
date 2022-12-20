## **Praktkumsaufgabe b)**

## **Aufgabenstellung:**
* Formulieren Sie einen (nicht-trivialen) Anwendungsfall Ihrer Wahl textuell mittels Interaktionsszenarien aus, wobei mindestens zwei Ausnahmeszenarien enthalten sein sollten.

## **Aufgabenbearbeitung:**

---
__USE-CASE "Auto reservieren (includes Auto suchen/finden)"__ <- Erste Idee

__Positivszenario - Idee 1:__ 

1. Kunde ruft die Suchfunktion auf 
2. System stellt mehrere Suchkriterien zur Verfügung (Standort, Zeitraum, Modell, Preis)
3. Kunde modelliert seine Suche nach gewünschten Kriterien
4. System prüft Angaben und zeigt Liste reservierbarer Autos nach den angegebenen Kriterien an
5. Kunde sucht sich passendes Fahrzeug aus und möchte dieses reservieren
6. System fragt nach dem gewünschten Zeitraum für die Reservierung
7. Kunde gibt den gewünschten Zeitraum der Reservierung ein
8. System prüft die Datumseingabe auf Gültigkeit
9. System fragt nach manueller Bestätigung der Reservierung
10. Kunde bestätigt die Reservierung
11. System bestätigt Reservierung durch Sendung einer Mail

ENDE

__Ausnahmeszenario 1 Reservierung in Vergangenheit: (nach Schritt 8 Positivszenario__

 "DATUM VOR "HEUTE""

__Ausnahmeszenario 2 Auto ist schon von jemanden reserviert: (nach Schritt 5 Positivszenario__

 "KUNDE BRAUCHT ZU LANGE FÜR ENTSCHEIDUNG"

---
__USE-CASE "Fahrzeugreservierung außerhalb des Zeitraums"__ <- Zweite Idee

__Positivszenario - Idee 2:__


__Ausnahmeszenario 1 Reservierung in Vergangenheit:__


__Ausnahmeszenario 2 Auto ist schon von jemanden reserviert:__

---
__USE-CASE "Kreditkarte kann nicht belastet werden"__ <- Dritte Idee

__Positivszenario - Idee 3:__

1. Abrechnung


__Ausnahmeszenario 1 Fehlerhaft eingegebene Kreditkartennummer:__


__Ausnahmeszenario 2 Keine ausreichende Liquidität vorhanden:__









