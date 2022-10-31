---
title: User-centric web experience - Nook 2022
separator: ---
verticalSeparator: -v-
revealOptions:
  transition: "slide"
---

<!-- npx reveal-md ./slides.md -->

# Data-driven UX

Core Web Vitals und das Rail performance Model

-v-

Moin 👋

Ich bin Jakob,  
und manchmal mache ich 1 WebDev.

-v-

Es gibt da dann ja so Komplexitäten, mit Software

- im Problem das wir lösen wollen
- in Browsern
- in der UI

-v-

Komplextät ist immer mal sehr verlockend.

(Wir denken uns dann was)

-v-

Angenehm kann dann auch sein

- eine gute Lösung zu bauen
- UI, die schwuppt
- Software, die Leute gerne benutzen

---

## UX

-v-

> The **user experience** (UX) is how a user interacts with and experiences a product, system or service …

[en.wikipedia.org/wiki/User_experience](https://en.wikipedia.org/wiki/User_experience)

> a user’s perceptions and responses that result from the use and/or anticipated use …

[ISO 9241](https://en.wikipedia.org/wiki/ISO_9241)

-v-

Ganz schöner Themenkomplex.

-v-

Wir gucken uns nur ein paar Aspekte an,  
Google tut da was:

- Core Web Vitals
- Das Rail performance model

-v-

Wir gucken uns nicht an:

- Viele Sachen
- A11y, aria, reduced-motion, high-contrast / low-contrast

-v-

### Hot take 🌶️

- Gute UX passiert nicht einfach so
- Es reicht nicht aus, auf Gutes zu hoffen
- Gute Software hat Methode
- Messen und verbessern von Mängeln
- Engineering culture

---

## Response times

-v-

Nielsen Norman Group (NN/g)

[www.nngroup.com/../response-times-3-important-limits/](https://www.nngroup.com/articles/response-times-3-important-limits/)
Auch: Miller 1968 - Response time in man-computer conversational transactions

-v-

Experimente:

- Messen von Intervallen, die von Menschen als klar länger/kürzer wahrgenommen werden
- Die Sache mit der Frustration beim Umblättern

-v-

Daraus hervorgegangen:
Empfehlungen von Zeitbudgets für typische Interaktionen mit Systemen.

Beispiele:

- Zeit bis zum Signalton am Telefon
- Frustrationen bei Interaktion mit textbasierten Interfaces
- Nebenläufige Prozesse - in 1h oder 1t ist ~egal

-v-

Viele Vermutungen, wenig Messungen

Behauptung, Miller 1968:
(Reaktions-)Zeiten sind allgemeingültig, verändern sich wenig

-v-

Nach wie vor Grundlage für viele Interfaces

Davon wurde auch ein spezifisches Performancebudget abgeleitet,
das RAIL modell

-v-

Akronym erklären

Budgets erklären

Zeiten für Frames ableiten

Zeiten für Idle/Load ableiten

---

## Das Rail modell

[web.dev/rail](https://web.dev/rail/)

---

Die Sache mit den Nummernblöcken
Deininger 1960 - Human factors engineering studies of the design and use of pushbutton telephone sets

-v-

Beim Wechsel von Wählscheiben zu Knöpfen an Telefonen waren viele Fragen offen:

- Was sind gute Verteilungen von Knöpfen in der Fläche?
  - Wie sollten diese Verteilungen beschriftet werden?
- Wie groß und mit welchen Abständen sollten Knöpfe verteilt sein?
- Wie sollten Knöpfe auf Druck reagieren?

-v-

Real User Data vs. Lab data

Idee: Tatsächliche Leute als möglich Nutzende zu Rate ziehen.

Datenerhebung:

- Korrektheit der Eingaben
- Eingabegeschwindigkeiten
- Ratschläge/Ansichten der Testenden in Textform

-v-

Ableiten von Web Vitals

Unterschied zwischen Lab Data und RUM
Was ist der Zugewinn durch RUM?

-v-

Was wird sich von diesen Metriken erhofft?

- Von Google
- Von Leuten, die Websites bauen
- Von Nutzenden

-v-

LCP - Largest Contentful Paint

Wie lange dauert es, die größte, initial sichtbare Fläche zu rendern?
Wir interessieren uns für das p75 der Messungen.

Kontext:
Das größte initiale Element - gleich ob Bild oder Text - einer Seite trägt den wichtigsten Inhalt.
Warten auf wichtige Inhalte ist frustrierend.

-v-

FID - First Input Delay

Wie lange ist die Verzögerung zwischen dem Auslösen der ersten Interaktion
  mit einer Seite und einer darauf folgenden Reaktion?
Wir interessieren uns für das p75 der Messungen.

Kontext:
Gerade Seiten mit JavaScript können besondere Verzögerungen bei Interaktionen haben.
Langsamere Verbindungen sind eine zusätzliche Last.
Initaler Delay -> ggf. passiert noch besonders viel zum Laden von Seitenteilen.

-v-

CLS

---

A draft on how to measure

sendBeacon
How to with Fastly
In case of Cloudflare just change the CDN ;)
S3 or similar

---

// We start with some introduction

The topic is big -> we only talk about aspects

UX is a big word and lots of things can be meant by it and included with it.
What does it mean for us here?

What are we focussing on?

- Stuff done by Google
- Core Web Vitals
- Rail model

Maybe: what are we leaving out of scope?
A11y aria reduced-motion high-contrast low-contrast

What are implications?

- For Google
- For the Web
- For users

CTA
Good stuff is not an accident
Good websites are engineered
Good engineering has a culture

---

Web Vitals
[web.dev/vitals](https://web.dev/vitals/)

What is the aim?
How is data gathered?
What is real-user data vs. lab data?

-v-

LCP FID CLS ..

UI patterns / anti-patterns

Demo of recording web vitals
Demo of measuring performance in Chrome

---

RAIL model
[web.dev/rail](https://web.dev/rail/)

Why have a performance model?
The idea of a budget that is derived from measured numbers.

---

- ⏱️ Lasst mal Dinge messen!
- 🚀 Lasst mal ungünstige Messungen besser machen!

Weil wir Software mögen und so 🤗

- Slides: [github.com/runjak/nook2022](https://github.com/runjak/nook2022)
- Website: [runjak.codes](https://www.runjak.codes/)
