## Layer_Accountability_Gap

**Kategorie:** Systemarchitektur / Interface
**Tags:** [ARCH] [INTERFACE] [CAUSAL]

**Beschreibung:**
In hochgradig geschichteten Software-Stacks ist kein einzelner Layer
für Fehler an Schichtübergängen verantwortlich. Jede Komponente
verhält sich spezifikationskonform, dennoch entsteht am Ausgang
fehlerhafter Output. Der Fehler existiert im Übergang, nicht im Layer.

**Beispiel:**
Gboard → Android Clipboard → App: Copy einer Tabelle ergibt `null`.
Jeder Layer "korrekt" — Fehler strukturell nicht zuordenbar.

**Verwandt:**
- Kausalitätsdefizit-Syndrom
- False_Positive_Symptom
- Interface_Ambiguity_Node

**Epikrise:**
Babel-Problem nicht der Sprachen, sondern der Verantwortungslücken.
Gegenmodell: vollständige Ketten-Übersicht (Z80-Prinzip).

Ergänzend für mich durch Claude Sonnet 4.6 #b0580611 #Computerakex