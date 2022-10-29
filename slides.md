---
title: User-centric web experience - Nook 2022
separator: ---
verticalSeparator: -v-
revealOptions:
  transition: 'slide'
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

Die Sache mit den Nummernblöcken

---

Die Sache mit den Delays

---

Das Rail modell

---

Diese Web Vitals

---

LCP

---

FID

---

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