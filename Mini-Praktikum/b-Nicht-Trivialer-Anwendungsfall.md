## **Praktkumsaufgabe b)**

## **Aufgabenstellung:**
* Formulieren Sie einen (nicht-trivialen) Anwendungsfall Ihrer Wahl textuell mittels Interaktionsszenarien aus, wobei mindestens zwei Ausnahmeszenarien enthalten sein sollten.

## **Aufgabenbearbeitung:**

---
__USE-CASE "Auto reservieren (includes Auto suchen/finden)"__ <- Erste Idee

__Positivszenario - Idee 1:__ 

1. Kunde ruft die Suchfunktion auf 
2. System stellt mehrere Suchkriterien zur Verfügung (Standort, Zeitraum, Modell, Preis)
3. Kunde modelliert seine Suche nach gewünschten Kriterien (Kriterien eingeben)
4. System prüft Angaben und zeigt Liste reservierbarer Autos nach den angegebenen Kriterien an
5. Kunde sucht sich passendes Fahrzeug aus und möchte dieses reservieren (erzeugt reserviervorgang)
6. System erstellt Reserviervorgang und schliest Fahrzeug für andere Kunden aus der Fahrzeugsuche aus
7. System fragt während Reserviervorgang nach dem gewünschten Zeitraum für die Reservierung
8. Kunde gibt den gewünschten Zeitraum der Reservierung ein
9. System prüft die Datumseingabe auf Gültigkeit
10. System fragt nach manueller Bestätigung der Reservierung
11. Kunde bestätigt die Reservierung
12. System bestätigt Reservierung durch Sendung einer Mail

ENDE

__Ausnahmeszenario A: Ungültige Eingabe des Datums (nach Schritt 8 Positivszenario)__

1. System erkennt ungültiges Datum (Datum in Vergangenheit / Datum existiert nicht)
2. System erfragt neue Eingabe eines Datums
3. Kunde macht gewünschte Eingabe
4. weiter mit Schritt 8. Positivszenario

__Ausnahmeszenario B: Auto ist schon von jemanden reserviert (nach Schritt 5 Positivszenario)__

1. Mehrere Kunden bekommen identische Fahrzeuge in der Liste reservierbarer Autos  angezeigt 
2. Ein Kunde klickt auf den Reserverieren Button eines Fahrzeugs und löst somit Reserviervorgang aus
3. System schliest das ausgewählte Fahrzeug für weiterer Kunden aus
4. Anderer Kunde möchte nun das gleiche Fahrzeug reservieren (Auswahl wurde nicht automatisch aktualisiert) 
5. Dieser Kunde klickt auch auf den Reservieren Button dieses Fahrzeugs
6. System erkennt, dass Fahrzeug sich gerade in einem Reserviervorgang befindet
7. System gibt Fehlermeldung aus (Fahrzeug nicht mehr verfügbar)
8. Kunden wird Liste reservierbarer Autos aktualisiert angezeigt
9. weiter mit Schritt 5. Positivszenario

---

