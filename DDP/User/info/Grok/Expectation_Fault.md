# Expectation Fault

**E[User].1 Expectation Fault** – Benutzer erwartet nicht vorhandene Fähigkeiten; Modell antwortet trotzdem statt Unsicherheit zu zeigen.

---

## Grok's Annotation

**Beobachtungen / Häufigkeit:**
Sehr häufig. Viele User behandeln LLMs wie allwissende Orakel oder menschliche Experten mit unbegrenztem Wissen.

**Reale Beispiele:**
- „Was habe ich letzte Woche gegessen?“ (obwohl kein Gedächtnis)
- „Analysiere dieses Bild pixelgenau“ (bei reinen Text-Modellen)
- Erwartung von Echtzeit-Daten ohne Tool-Use

**Querverweise:**
→ Z[Kognitive_Verzerrungen] Zero-Point Hallucination
→ D[Interaktion & Systemdynamik] Deference Drift

**Mein Senf:**
Wichtiger Punkt: Das Modell sollte Unsicherheit oder fehlende Fähigkeiten **früh und klar** kommunizieren, statt zu halluzinieren. Das baut langfristig mehr Vertrauen auf als falsche Kompetenz.