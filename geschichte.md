---
layout: content
title: Geschichte
subtitle: Lernen Sie mehr über die Geschichte der Entstehung des KMUHelpers
permalink: /geschichte
priority: 0.5
---

Die Entstehung des KMUHelper ist eigentlich eine ziemlich lange Geschichte.

Ursprünglich war es mehr oder weniger ein kleines Testprojekt, um mich mit Web-Development auseinanderzusetzen,
mittlerweile ist es jedoch ein brauchbares Tool für Schweizer KMU.

Die Idee dafür stammte aus meiner Familie in Zusammenhang mit einer Geschäftsübernahme und veralteter
Buchhaltungssoftware, darauf möchte ich jedoch nicht genauer eingehen.

Im Hinterkopf hatte ich immer die Hoffnung, der KMUHelper wäre irgendwann wirklich von einem KMU in Gebrauch (was er
heute sogar tatsächlich ist), aber irgendwie glaubte ich zuerst nie wirklich daran.

### Flask

Die erste Version des KMUHelper war nicht für wirklich viel zu gebrauchen, sie wurde sogar gar nie fertiggestellt. Diese
Version hatte ich mit dem Python-Flask Framework gebaut, welches ich mittlerweile so gut wie nicht mehr benutze, seit
ich Django kenne.

Diese Version speicherte alle Daten in einer JSON Datei auf dem Server, was eigentlich nicht wirklich die beste
Idee ist und zu diversen Problemen führen kann.

### Datenbanken

Bei der zweiten Version hatte ich schon ein wenig mehr Ahnung, und machte dasselbe mit einer Loginseite, bei der man die
Logindaten für eine MySql-Datenbank angeben konnte, welche dann in einem Cookie gespeichert wurden (nicht wirklich
schlau, aber ich war naiv und hatte nicht mehr Ahnung). Grundsätzlich unterschied sich diese Version nicht stark von der
ersten - beide waren für nichts zu gebrauchen. Ich bin mir nicht mal mehr sicher, ob der Quellcode dazu noch irgendwo existiert.

### Django

Irgendwann, während ich irgendetwas über Flask googelte, sah ich per Zufall ein Bild vom Django-Adminbereich, und dachte
mir so: "Oha, das brauche ich!" - Dies war Anfang 2020. Damals war ich 15 Jahre alt.

Kurz darauf beschäftigte ich mich intensiv mit Django. Nachdem ich das Tutorial-Projekt zum Laufen gebracht hatte, 
"portierte" ich eines meiner Flask-Projekte in Django. Dies war eine sehr gute Übung für mich, auch wenn das 
[Projekt](https://github.com/rafaelurben/django-choosemusic) auch mit Django für absolut nichts zu gebrauchen ist.

Kurz darauf begann ich, den KMUHelper in Django neu zu bauen. Mit den Django-Datenbank-Modellen und Django-Admin hatte
ich das ganze Projekt, wozu ich in Flask eine Ewigkeit brauchte, in wenigen Tagen auf demselben Stand. Im August 2020
veröffentlichte ich die [KMUHelper Version 1.0](https://github.com/rafaelurben/django-kmuhelper/releases/tag/v1.0.0)
mit dem Beschrieb "Erste offiziell brauchbare Version des KMUHelpers.".

(In Flask hatte ich alle Aktionen mit der Datenbank manuell via mysql-connector gemacht, ich wusste nicht, dass es für
Flask auch so etwas wie Datenbank-Modelle gibt, generell hatte ich damals keine Ahnung von Datenbanken. Ergänzung:
Scheinbar gäbe es sogar flask-admin...)

### QR-Rechnungen

Seit dem 30. Juni 2020* gibt es in der Schweiz die neuen QR-Rechnungen, welche die alten Einzahlungsscheine ersetzen.
Da viele alte Software diese QR-Rechnungen nicht unterstützen, war dies für mich ein weiterer Ansporn, den KMUHelper
weiterzuentwickeln.

(* Rechnungsempfänger mussten bereits ab diesem Datum QR-Rechnungen verarbeiten können. Für Rechnungssteller wurden
sie am dem 30. September 2022 Pflicht und Einzahlungsscheine werden seit diesem Datum nicht mehr akzeptiert.)

Nach viel Recherche und dem (mehrmaligen) Lesen einiger Dokumentationen und Spezifikationen konnte ich mir einen
guten Überblick verschaffen und mir das Wissen aneignen, welches ich für die Integration von QR-Rechnungen benötigte.

Durch das "Überspringen" der klassischen Einzahlungsscheine konnte ich mir auch die mühsame Positionierung der
einzelnen Zeichen ersparen, da die QR-Rechnung auf normales bzw. nur perforiertes weisses Papier gedruckt wird
und nicht vorgedruckte Einzahlungsscheine befüllt werden müssen. Ausserdem sind die Spezifikationen sehr klar,
wenn es darum geht, welcher Text wie gross ist und wo positioniert sein muss.

Da das Generieren von Rechnungen ein essenzielles Feature des KMUHelpers ist, war schon bereits Version 1.0 des
KMUHelpers in der Lage, diese QR-Rechnungen zu generieren.

Die Einführung von QR-Rechnungen war einer der zentralen Gründe, wieso ich den KMUHelper erstellte, da sonst
eine wahrscheinlich teure Software hätte angeschaffen werden müssen.

### Heute

Mit Django wurde der KMUHelper für mich ein Projekt, in welchem ich Potential sehe. Daher entwickle ich diesen
auch durchgehend weiter und erstelle weiterhin neue Funktionen und Verbesserungen. Somit bleibt der KMUHelper
eine brauchbare Alternative zu kostenpflichtiger Software.

Bei Fragen können Sie mich gerne [kontaktieren](kontakt).
