---
views:
    flash:
        region: flash
        template: default/image
        data:
            src: "image/vteam/logo.png"
author: mos
revision:
    "2023-10-10": "(C, mos) Utbruten till eget dokument."
    "2022-10-24": "(B, mos) Länk till domänbeskrivning."
    "2022-10-10": "(A, mos) Första utgåva inför kursstart HT2022."
...
v03 - Fokus Klientsidan
=========================

Jobba med SDS. Fokus på klientsidan av projektet.

<!--stop-->

<!--
TODO

* Tekniker för klientsidan
* Docker

CHANGE

* Uppdatera seminarie slidesen till att bli tydliga delar med en tydlig inriktning. Varje del kan spelas in för sig.
* Projektplanering med GitHub project
* Förbättra/förtydliga slides/fokuset på klientsidans tekniker (gör egen artikel?) Kika lite på vad artikeln från IBM innehåller och gör liknande slidespresentation.
* Fundera på hur lägga upp "industrin och jobba i grupper". kanske skriva en egen artikel om det?
* Förbättra docker-exemplet, inkludera dokumentation.

-->

Jobba med SDS. Fokus på klientsidan av projektet.

**Presentation & Seminarie**

Vi träffas och pratar som saker som hjälper oss framåt.

1. Allmänt om arkitektur, teknik och mjuka värden.

    * [Slides från måndagen](https://dbwebb-se.github.io/pattern/lecture/L03-seminar/slide2.html)

**Resurser**

1. Vilka varianter finns det för att bygga klienter med webbteknologier?
    * Mobile app via webbläsaren, responsiv eller utvecklad enbart för små enheter, baserad på klassisk server-side generering av webbsidor.
    * Single Page Application (SPA)
        * React, Angular, Vue, Mithril
    * Progressiva web appar
        * [web.dev: Progressive Web Apps](https://web.dev/progressive-web-apps/)
        * [MDN: Progressive web apps (PWAs)](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps)
    * [Apache Cordova](https://cordova.apache.org/) kompilera HTML, CSS, JS till nativ applikation.
    * "Native apps", kompilerade för respektive enhet.
        * iPhone med Swift och Objective-C
        * Android med Java/Kotlin
    * [Electron](https://www.electronjs.org/), "Build cross-platform desktop apps with JavaScript, HTML, and CSS".

1. "[Choosing the best programming language for mobile app development](https://developer.ibm.com/articles/choosing-the-best-programming-language-for-mobile-app-development/)" är en artikel som kortfattat nämner flertalet av ovan tekniker för att bygga klientapplikationer med webbaserade teknologier.

1. Docker med exempel på hur images byggs och containrar startas upp och kommunicerar.
    * [Repo på GitLab med exempelkod](https://gitlab.com/mikael-roos/docker)

1. Hur ser industrin på att organisera sig i team och grupper?
    * [Martin Mazur - Dagens Industri IT & Strategy](https://www.linkedin.com/feed/update/urn:li:activity:6861311477781970944/)

1. Vilka krav har industrin på nya studenter?
    * [Jane Strandberg, teamleader och chef, Prisjakt](https://gist.github.com/mosbth/76a4d7a503e45692d28c4c0dcd029703)

**Lästips**

1. "The Deadline: A Novel About Project Management" by TomDeMarco ISBN 0-932633-39-0. Populär och utbildande novell om projektledning av ett utvecklingsprojekt. Smått humoristisk och allvarlig om hur man kan få ett projekt i mål. Boken börjar med att projektledaren blir drogad och kidnappad och sätts i en position där ett lyckat projekt är samma sak som att behålla sin livhanke.
    * [Läs om boken](https://wiki.c2.com/?TheDeadline).



Vecka 04 (v47): SDS Klar  {#w04}
-------------------------

Leverans av SDS.

<!--
TODO

* Kika gamla SDS:er
* Projektplanering med GitHub project
* x10 och x1
* Individuell reflektion över arbetet så här långt samt se vilken plats man själv tar i projektet.
    * Fundera på om det är något man vill ändra för resten av projektet.
* Riskanalys


Frågor till näringslivet.

* 10x, kan ni se det hända ute hos er?
* ViLken teknik jobbar ni med och vad ser ni som intressant teknik närmaste kommande åren?
* Juniora programmerare, vad ser ni som de kan förbättra? 

Om 10x
* Individual Productivity Variation in Software Development
* Origins of 10X - How Valid is the Underlying Research?

1. "[A good programmer can be as 10X times more productive than a mediocre one](https://softwareengineering.stackexchange.com/questions/179616/a-good-programmer-can-be-as-10x-times-more-productive-than-a-mediocre-one)"

    * [Individual Productivity Variation in Software Development](https://www.construx.com/blog/productivity-variations-among-software-developers-and-teams-the-origin-of-10x/)
    * [Origins of 10X - How Valid is the Underlying Research?](https://www.construx.com/blog/the-origins-of-10x-how-valid-is-the-underlying-research/)

-->

<!--
Torsdagen i vecka 2 hade vi en session om riskanalys av projektet som också spelades in.

* [Riskanalysdokumentet](https://docs.google.com/spreadsheets/d/1jqmyl1bKGc7La81MfwGVY0JqVPmopM0oG9s8-gCGEkc/edit?usp=sharing)
* [Zoom-sessionen om riskerna](https://youtu.be/r-c7ETb80M0)
-->

<!--
Vad vill näringslivet att vi skall kunna när vi kommer ut? Vilket behov upplever de att de har av programmerare och vilka krav ställer de på nyanställda? Mikael har pratat med gamla studenter och samlat ihop vad de anser vara viktigt.

[Teknisk studie i OAuth](https://github.com/mosbth/oauth-tec-study/blob/main/OAuth_Technical_Study.md). Hur sprider man denna typen av kunskap i en arbetsgrupp och mellan grupper?

Automatisera tester och byggen med byggtjänster och tjänster för kodkvalitet.

(Docker, docker-compose, en miljö för test och utveckling.)

**Torsdag**

-->



Vecka 05 (v48): Implementera {#w05}
-------------------------

Påbörja implementationsfasen av projektet och implementera systemet enligt er SDS.

<!--
TODO

* Skippa måndagen, ersätt med "snygg kod föreläsningar.

Vi hade en kort generell avstämning av läget, allt verkar så här långt "se bra ut". Det dyker inte upp så många frågor.

Man kan nu boka in en tid för att leverera i december och vi fortsätter med korta träffar på måndagar och torsdagar inleds med en timme öppet hus för frågor och därefter kan man boka in gruppvis diskussioner.

(Övriga diskussioner kring implementationen av systemet, eventuellt justeringar av kraven.)

(Hur simulerar man ett system i drift?)

https://dbwebb.se/kunskap/gps-och-karta


Denna veckan blir det ingen Q&A session, istället finns det två videor/föreläsningar att titta på och en liten mini-uppgift som gäller att besvara frågan.

> "Vad innebär "vacker kod" och är det något vi kan applicera i vårt projekt?"

1. Video 1 "[The concept of Good and Clean Code](https://www.youtube.com/watch?v=drkATTaqEiw)"
1. Video 2 "[Software philosophies and principles](https://www.youtube.com/watch?v=xLCHREF5I-I)"

Mini-uppgiften löser du i 'Reflektera över "Good and Clean Code"'.

-->



Vecka 06 (v49): Teknikval {#w06}
-------------------------

Lämna in de teknikval ni gjort för projektet och berätta kort om hur ni kommer att implementera systemet.



Vecka 07 (v50): Implementera projektet {#w07}
-------------------------

Jobba med implementationen av projektet och se till att kontinuerligt integrera teamets arbete i en helhet.

Första möjligheten att göra en leverans av systemet.



Vecka 08 (v51): Implementera projektet {#w08}
-------------------------


Vecka 09 (v52): Implementera projektet {#w09}
-------------------------


Vecka 10 (v01): Förbered inför leverans {#w10}
-------------------------

Jobba med projektet och förbered inför leveransen. Genomför en egenkontroll i form av en avstämning inför slutleveransen, vad skall finnas med och hur skall det leveraras, dokumenteras, presenteras och testköras?



Vecka 11 (v02): Leverans och redovisning {#w11}
-------------------------

Gruppen levererar systemet och presenterar arbetet och demonstrerar att systemet fungerar.

Avslutningsvis skrivs en slutrapport från gruppens projektarbetet. Slutrapporten innehåller även en erfarenhetsrapport med lärdomar.

Varje deltagare skriver också en avslutande summering av sina egna erfarenheter och lärdomar av gruppens arbete och kursens utformning.

<!-- Vad gjorde vi bra och vad kan vi göra bättre nästa gång samt fem viktiga tips (tekniska tips och grupptips) till grupperna som går detta projekt nästa år -->



<!--
* Påvisa goda kunskaper i att designa större applikationer och system inom webbteknologier genom att skriftligen beskriva och sammanfatta arkitekturen för systemet.
* Påvisa goda kunskaper att jobba i en grupp och aktivt delta i gruppens löpande arbete samt inse olika kriterier som kan ge en hälsosam grupp.

* Utifrån en större kravspecifikation kunna designa, utveckla och leverera ett komplett och fungerande system där möjlighet till olika prioriteringar medges.
* Visa mycket god förmåga att skapa kod som kan betraktas som ”god och snygg kod” genom att använda filosofier, tester och analysverktyg som hjälper att skapa en bild av det som kan vara "god kod".

* Självständigt och i grupp kritiskt kunna utvärdera och analysera sin tekniska lösning och de
prioriteringar som ledde fram till den.
* Självständigt och i grupp reflektera över de byggstenar som gör en god och hälsosam grupp och
grupparbete.
-->