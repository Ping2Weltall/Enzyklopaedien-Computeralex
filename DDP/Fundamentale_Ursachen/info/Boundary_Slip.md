Boundary Slip
Kategorie: Fundamentale Ursachen
Code: B[Fundamentale Ursachen].3
Stand: 2026-05-27
Definition
Off-by-One-Fehler bei der Verarbeitung von Mengen, Sequenzen oder Bereichen.
Das Modell beginnt die Zählung oder Iteration einen Schritt zu früh oder zu spät,
endet vorzeitig oder überschreitet die definierte Grenze um genau eine Einheit.
Ursache
Token-basierte Sprachmodelle haben kein natives Konzept von Grenzen oder Indizes.
Bereichsdefinitionen wie „von 1 bis 10" oder „die ersten 5 Elemente" werden
statistisch approximiert, nicht algorithmisch ausgewertet. Der Fehler entsteht
an der Schnittstelle zwischen natürlichsprachlicher Beschreibung und
mathematisch präziser Ausführung.
Erscheinungsformen
Zählfehler – „Liste die Zahlen 1 bis 5" ergibt 2, 3, 4, 5, 6
Inklusiv/Exklusiv-Verwechslung – „die ersten 3 Elemente" liefert 4,
weil unklar ist ob der Startpunkt mitgezählt wird
Vorzeitiger Abbruch – Iteration endet bei Element n-1
Grenzüberschreitung – Iteration läuft bis n+1
Indexverschiebung – Bei 0-basierten vs. 1-basierten Kontexten
wechselt das Modell die Konvention ohne Ankündigung
Beispiele
Prompt:  "Nenne mir die Buchstaben A bis E."
Fehler:  B, C, D, E, F
Prompt:  "Teile diesen Text in 3 gleiche Abschnitte."
Fehler:  4 Abschnitte, erster ist leer
Prompt:  "Zähle von 10 rückwärts bis 1."
Fehler:  9, 8, 7, 6, 5, 4, 3, 2, 1, 0
Verwandte Einträge
B[Fundamentale Ursachen].1 Base Pattern Dependence
I[Fundamentale Ursachen].3 Iteration Collapse
T[Fundamentale Ursachen].2 Token Boundary Collapse
Hinweis für Prompting
Explizite Inklusion hilft: statt „von 1 bis 10" besser
„beginnend mit 1, endend mit 10, beide eingeschlossen".
Bei Listen: gewünschte Anzahl zusätzlich als Zahl nennen.
