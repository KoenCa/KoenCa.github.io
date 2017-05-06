---
layout: post
title: Introduction to integration with Apache Camel
subtitle: Pluralsight cursus
bigimg: /img/apache-camel.jpg
tag: levenslang_leren
---

Voor mijn stage moet ik veel nieuwe technologieën/frameworks bijleren. Eén van deze frameworks is Apache Camel waarvoor ik een online cursus heb gevolgd op Pluralsight. In dit verslag zal ik voor deze cursus per hoofdstuk een korte beschrijving geven met op het einde een korte reflectie.

## Hoofdstuk 1: Introduction to enterprise integration
In dit hoofdstuk van de cursus werd uitgelegd wat Enterprise Integration is, omdat dit belangrijk is voor het verdere verloop van de cursus en Apache Camel is een framework wat het veel makkelijker maakt om hiermee te kunnen werken. Het mediator design pattern waar Camel gebruik van maakt werd hier ook uitgelegd aan de hand van een voorbeeld. Voor dat ik aan deze cursus begon had ik al wat opgezocht over Enterprise Integration,maar dit was nog een mooie herhaling voor mij. Dat Apache Camel het Mediator design pattern gebruikt was wel nieuw voor mij en dit is goed om te weten.

## Hoofdstuk 2: Getting started with Apache Camel
Bij dit hoofdstuk word de demo code verder uitgelegd die doorheen de cursus gebruikt gaat worden. Zelf had ik problemen om de PostgreSQL database aan te maken, omdat de scripts van de cursus fouten geven bij mij. Ik heb hier redelijk wat tijd in gestoken om dit uit te zoeken, maar ik heb het niet kunnnen oplossen. Om niet nog meer tijd erin te steken heb ik besloten om verder te gaan met de cursus zonder de database dan. 

Verder werd er in dit hoofdstuk nog een codevoorbeeld geschreven van een Camel route. Dit was een simpele route om bestanden wat in een bepaalde map komen te verplaatsen naar een andere map. Dit met maar een paar lijnen code, wat normaal meer zou zijn om dit goed te kunnen laten werken. Dit is natuurlijk de bedoeling van een framework om het je een stuk makkelijker te maken.

## Hoodstuk 3: Routing from a database
In dit hoofdstuk werd de kracht van Apache Camel nog duidelijker. Er werd getoond hoe je met een paar lijnen code bepaalde wijzigingen in de database kon opvangen om daarna er iets mee te doen. Bij deze demo werden nieuwe bestellingen in de database verwerkt door hun status aan te passen en deze dan te loggen in een logbestand. Voor deze functionaliteit werd er ook een unit test geschreven om de route te testen.

## Hoofdstuk 4: Message processing
In de vorige hoofdstukken werd er vooral met routes gewerkt in Apache Camel. Nu werd het volgende grote onderdeel van Apache Camel besproken namelijk messaging. Camel maakt gebruik van het Message Enterprise Integration Pattern en in dit hoofdstuk werd dit ook verder uitgelegd hoe Camel dit precies implementeerd.
Na de meer theoretische uitleg werd dit ook weer in de praktijk toegepast in de demo code. De route van vorig hoofdstuk werd hierbij uitgebreid om de gegevens die uit de databse gehaald worden om te zetten naar XML. Deze XML messages werden dan weer doorgestuurd naar de logging.

## Hoofstuk 5: Routing to a JMS Queue
In dit hoofdstuk word de route van de vorige hoofdstukken uitgebreid met een Java Messaging Service (JMS). JMS werd eerst kort uitgelegd voor dat deze geïmplementeerd werd in de demo code. Voor de implementatie van de JMS API werd er gebruikt gemaakt van een ActiveMQ server. De uitbreiding van de route zorgde ervoor dat de messages met data uit de database doorgestuurd werden naar de ActiveMQ server.

## Hoofdstuk 6: Content based router
In dit hoofdstuk word er een nieuwe route met een content based router toegevoegd. Deze router zorgt ervoor dat de messages die door de andere router aangemaakt waren op de juiste bestemming aankomen. Deze routing is ook weer geïmplementeerd door middel van een paar lijnen code die lijken op een switch case van Java.

## Hoofdstuk 7: Routing to a web service
In dit hoofdstuk werd er getoond hoe je de messages door kan sturen naar een REST API. In de demo code werd er een nieuwe route aangemaakt die dit mogelijk maakte. Deze route zorgt er ook voor dat de XML body van de message eerst word omgezet naar een JSON body, om dat de REST API enkel JSON accepteert. 

## Hoofdstuk 8: Routing with SFTP
Het laatste hoofdstuk van deze cursus en ook een van de meest uitgebreide. Er word een nieuw Enterprise Integration Pattern besproken namelijk Aggregator. Er werden ook nog drie nieuwe Camel componenten besproken namelijk: CSV component, file component en het FTP component. Op het einde van dit hoofdstuk werd ook nog kort error handling besproken in Apache Camel. Deze onderwerpen werden ook allemaal aangemaakt in de demo code via Test Driven Development. Er werden eerst testen voor de routes geschreven en daarna pas de echte functionaliteit voor de routes.

## Reflectie
Ik ben aan deze cursus begonnen, omdat ik Apache Camel moet gebruiken in mijn stageopdracht. Door deze cursus te volgen snap ik Apache Camel weer een beetje beter. Er zijn veel verschillende componenten besproken in deze cursus samen met een simpele implementatie in de demo code waardoor ik nu een mooie basis heb om mee te beginnen. Nu na deze cursus ben ik van plan om verder te gaan met meer praktische tutorials waar ik zelf Apache Camel projecten zal bouwen.

In het algemeen vond ik dit een goede cursus om de basis te leren van Apache Camel. Soms was de code in de videos wat onduidelijk, maar dan keek ik zelf even in de demo code om het wat duidelijker te maken. Deze cursus heeft mij een goede basis gegeven om nu nog zelf verder dingen op te zoeken over Apache Camel en meer praktische ervaring op te doen.
