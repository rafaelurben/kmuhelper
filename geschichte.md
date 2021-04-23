---
layout: content
title: Geschichte
subtitle: Lernen Sie mehr über die Geschichte der Entstehung des KMUHelpers
permalink: /geschichte
priority: 0.5
---

Die Entstehung des KMUHelper ist eigentlich eine ziemlich lange Geschichte.

Ursprünglich war es mehr oder weniger ein kleines Testprojekt, um mich mit Web-Development auseinanderzusetzen, mittlerweile ist es jedoch ein brauchbares Tool für die Buchhaltung von Schweizer KMU.

Die Idee dafür stammte aus meiner Familie in Zusammenhang mit einer Geschäftsübernahme und veralteter Buchhaltungssoftware, dazu möchte ich jedoch nicht genauer eingehen.

Im Hinterkopf hatte ich immer die Hoffnung, der KMUHelper wäre irgendwann wirklich von einem KMU in Gebrauch (was er heute sogar tatsächlich ist), aber irgendwie glaubte ich nie wirklich daran.

### Flask

Die erste Version des KMUHelper war nicht für wirklich viel zu gebrauchen, sie wurde sogar gar nie fertiggestellt. Diese Version hatte ich mit dem Python-Flask Framework gebaut, welches ich mittlerweile so gut wie nicht mehr benutze, seit ich Django brauche.

Ich weiss nicht, was ich mir damals überlegt habe, aber diese Version speicherte alle Daten in einer JSON Datei auf dem Server, was eigentlich nicht wirklich die beste Idee ist.

### Datenbanken

Bei der zweiten Version hatte ich schon ein wenig mehr Ahnung, und machte dasselbe mit einer Loginseite, bei der man die Logindaten für eine MySql-Datenbank angeben konnte, welche dann in einem Cookie gespeichert wurden. Grundsätzlich unterschied sich diese Version nicht stark von der ersten - beide waren für nichts zu gebrauchen. Den Quellcode dazu habe ich noch irgendwo, aber jetzt mal ehrlich, das will niemand sehen... Quellcode unerfahrener Programmierer... Ich bekomme schon fast Kopfschmerzen, wenn ich mir den ansehe.

### Django

Irgendwann, während ich irgendetwas über Flask googelte, sah ich per Zufall ein Bild vom Django-Adminbereich, und dachte mir so: "Oha, das brauche ich!"

Kurz darauf beschäftigte ich mich intensiv mit Django und, nachdem ich das Tutorial-Projekt zum Laufen gebracht hatte, "portierte" ich eines meiner Flask-Projekte in Django ([Hier](https://github.com/rafaelurben/django-choosemusic) ist der Müll noch zu finden. xD). Dies war eine sehr gute Übung für mich, auch wenn das Projekt für absolut nichts zu gebrauchen ist.

Kurz darauf begann ich, den KMUHelper in Django neu zu bauen. Mit den Django-Datenbank-Modellen und Django-Admin hatte ich das ganze Projekt, wozu ich in Flask eine Ewigkeit brauchte, in wenigen Tagen auf dem selben Stand. (Ja, in Flask hatte ich alle Aktionen mit der Datenbank manuell via mysql-connector gemacht, ich wusste nicht, dass es für Flask auch so was wie Datenbank-Modelle gibt, generell hatte ich zuvor keine Ahnung von Datenbanken. xD EDIT: Scheinbar gibt es sogar flask-admin... o.O)

Mittlerweile ist der KMUHelper eine brauchbare, auf django-admin basierende Web-Applikation, welche sogar Schweizer QR-Rechnungen generieren kann. Die Einführung von QR-Rechnungen war übrigens auch einer der Gründe, wieso ich den KMUHelper erstellte.

### Heute

Mit Django wurde der KMUHelper für mich ein Projekt, in welchem ich Potential sah, da Buchhaltungssoftware für viele KMU viel zu teuer ist, und dies eine meiner Meinung nach gute Alternative zu konstenpflichtiger Buchhaltungssoftware ist. Klar, professionell ist er nicht wirklich, aber funktioniert tut er.
<!-- (Wenn ich nicht wieder mal mehr Bugs als Features erstelle... xD) -->

Dies ist natürlich nicht die ganze Geschichte, aber immerhin ein kleiner Überblick.

Bei Fragen können Sie mich gerne [kontaktieren](kontakt).
