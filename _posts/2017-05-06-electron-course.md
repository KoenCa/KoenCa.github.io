---
layout: post
title: 'Master Electron: Desktop Apps using HTML, JavaScript & CSS'
subtitle: Udemy cursus
bigimg: /img/electron-course.jpeg
tag: levenslang_leren
---

Deze cursus gaat over Electron. Dit is een framework waarmee je desktopapplicaties kan bouwen door gebruik te maken van HTML, JavaScript en CSS. Deze applicaties zijn compatibel met alle bekende platformen zoals Linux, Mac en Windows. Met Electron kan je dus je bestaande kennis van web developing gebruiken om desktopapplicaties te ontwikkelen. Dit is ook het meeste bekende framework hiervoor, want er zijn al veel bekende applicaties mee gemaakt zoals de tekst editors Visual Studio Code en Atom, ook de bekende chatapplicatie Slack is ontwikkeld met Electron. Je kan ook je favoriete JavaScript framework waar je misschien al veel ervaring mee hebt blijven gebruiken wat ook weer voordelig is. Deze cursus bestaat uit acht secties waarvan ik elke zal bespreken in dit verslag. 

Met deze cursus wil ik leren hoe je desktopapplicaties kan ontwikkelen door gebruik te maken van HTML, CSS en JavaScript. Dit lijkt me zeer interessant, omdat je op die manier bijna elk soort van applicatie kan ontwikkelen met deze drie technologieën.

## Sectie 1: Overview
Dit is een korte sectie waarin de lector vertelt hoe de rest van de cursus zal verlopen. Eerst zal de ontwikkelomgeving opgezet worden om op een efficiënte manier te werken met Electron. Hierna zal de Electron API bekeken en gebruikt worden zodat elke module van Electron duidelijke uitgelegd kan worden. Wanneer de API volledig doorlopen is zullen meer geavanceerde kenmerken en technieken van Electron uitgelegd worden. Hierbij zal ook gekeken worden hoe je Electron applicaties goed kan beveiligen. Om de cursus af te sluiten wordt al deze kennis gebruikt om een project te maken met Electron.

Voor elke sectie wordt ook het Electron starter project gebruikt dat terug te vinden is via de site van Electron of via de volgende GitHub repository:

 <a href="https://github.com/electron/electron-quick-start" target="_blank">Repository</a>

## Sectie 2: Developing with Electron
Dit is een meer algemene sectie waarin de lector verschillende tools en technieken laat zien die het makkelijker maken om te ontwikkelen in Electron. De lector laat ook zien hoe je de dependencies installeert en hoe je de applicatie start via NPM. De structuur van het starter project wordt ook verder uitgelegd. Dit is ook hoe de meeste Electron applicaties werken.

### Electron-reload
Dit is een third party node module die het ontwikkelen in Electron productiever maakt door de applicatie te herladen als je de code wijzigt. Zo hoef je zelf niet heel de tijd je applicatie opnieuw op te starten tijdens het ontwikkelen.

### Devtron
Uitbreiding van de standaard chrome developer tools die aanwezig zijn in een Electron applicatie. Devtron bied extra tools die specifiek ontworpen zijn voor Electron applicaties. Deze kunnen helpen bij het vinden van fouten of het toepassen van best practices tijdens het ontwikkelen. 

### Native node modules
Bij het ontwikkelen van een Electron applicatie kan er ook gebruik gemaakt worden van node modules zoals bcrypt voor het encrypteren van wachtwoorden. Het probleem is dat deze niet rechtstreeks gebruikt kunnen worden in Electron. De lector laat zien hoe je dit probleem kan oplossen door gebruik te maken van een script van de Electron website.

## Sectie 3: Main Process API
Een Electron applicatie bestaat uit drie delen die samen werken:

- Main Process API
- Render Process API
- Shared API

In deze cursus worden van elk deel de belangrijkere kenmerken besproken en uitgelegd aan de hand van code voorbeelden. In deze sectie gaat het over de Main Process API. Dit proces runt de main file van een Electron applicatie. Deze is altijd gespecifieerd in het package.json bestand. Het Main Process beheert alle venster van een Electron applicatie en handelt ook tal van events hiervoor af. 

In deze sectie worden alle klasses van deze API kort besproken. Dit zijn de volgende klasses:

- App: <a href="https://electron.atom.io/docs/api/app/" target="_blank">documentatie</a>
- BrowserWindow: <a href="https://electron.atom.io/docs/api/browser-window/" target="_blank">documentatie</a>
- Session: <a href="https://electron.atom.io/docs/api/session/" target="_blank">documentatie</a>
- Dialog: <a href="https://electron.atom.io/docs/api/dialog/" target="_blank">documentatie</a>
- Accelerator: <a href="https://electron.atom.io/docs/api/accelerator/" target="_blank">documentatie</a>
- GlobalShortcut: <a href="https://electron.atom.io/docs/api/global-shortcut/" target="_blank">documentatie</a>
- Menu: <a href="https://electron.atom.io/docs/api/menu/" target="_blank">documentatie</a>
- MenuItem: <a href="https://electron.atom.io/docs/api/menu-item/" target="_blank">documentatie</a>
- Tray: <a href="https://electron.atom.io/docs/api/tray/" target="_blank">documentatie</a>
- PowerMonitor: <a href="https://electron.atom.io/docs/api/power-monitor/" target="_blank">documentatie</a>

Voor elke klasse toont de lector een kort voorbeeld in de code. In sommige video’s gaat de lector wel wat snel, maar de functionaliteiten van elke klasse is ook best voor de hand liggend als je zelf even de documentatie bekijkt.

## Sectie 4: IPC Communication
Dit is een korte sectie met maar 1 video over IPC Communication. IPC staat voor Inter-Process Communication. Dit wordt in Electron gebruikt voor de communicatie tussen het Main Process en Renderer Process. Elk venster in een Electron applicatie is een object van de klasse BrowserWindow. Elk venster heeft ook zijn eigen Renderer Process dat soms moet communiceren met het Main Process om data door te geven. Hiervoor wordt het IPC-principe gebruikt in Electron. Dit is een belangrijk gedeelte van elke Electron applicatie, omdat dit alle aparte delen in de applicatie met elkaar verbindt. Beide processen hebben ook hun eigen klasses voor IPC namelijk ipcMain en ipcRenderer. 

De lector legt IPC op een simpele en duidelijke manier uit aan de hand van code voorbeelden en de documentatie op de Electron website. 

- <a href="https://electron.atom.io/docs/api/ipc-main/" target="_blank">Documentatie ipcMain</a>
- <a href="https://electron.atom.io/docs/api/ipc-renderer/" target="_blank">Documentatie ipcRenderer</a>

## Sectie 5: Renderer Process API
In deze sectie legt de lector het Renderer Process van Electron uit. Net zoals de sectie over het Main Process overloopt hij alle klasses die deel uit maken van het Renderer Process met korte voorbeelden. Dit proces is minder uitgebreid maar werkt wel nauw samen met het Main Process. In een Electron applicatie is er meestal wel maar één Main Proces en meerdere Renderer processen.

Het Renderer proces bevat volgende klasses:

- Remote: <a href="https://electron.atom.io/docs/api/remote/" target="_blank">documentatie</a>
- BrowserWindowProxy: <a href="https://electron.atom.io/docs/api/browser-window-proxy/" target="_blank">documentatie</a>
- WebFrame: <a href="https://electron.atom.io/docs/api/web-frame/" target="_blank">documentatie</a>
- Webview tag: <a href="https://electron.atom.io/docs/api/webview-tag/" target="_blank">documentatie</a>

Dit was ook weer een korte maar duidelijke sectie zoals de vorige secties. Enige probleem dat ik soms ondervind is dat de lector wat snel gaat, maar dan kan ik altijd even terugspoelen.

## Sectie 6: Shared API
Deze sectie gaat over het derde en laatste deel van Electron namelijk de Shared API. De Shared API is gewoon een verzamelnaam voor klasses die beschikbaar zijn in het Renderer Process en Main Process. Vandaar ook de naam ‘Shared’. Dit zijn de volgende klasses:

- Process: <a href="https://electron.atom.io/docs/api/process/" target="_blank">documentatie</a>
- Screen: <a href="https://electron.atom.io/docs/api/screen/" target="_blank">documentatie</a>
- Shell: <a href="https://electron.atom.io/docs/api/shell/" target="_blank">documentatie</a>
- NativeImage: <a href="https://electron.atom.io/docs/api/native-image/" target="_blank">documentatie</a>

Net zoals de vorige sectie was deze ook weer kort en duidelijk met hetzelfde probleem dat de lector soms wat snel is.

## Sectie 7: Features & Techniques
In deze sectie laat de lector nog wat technieken zien die handig kunnen zijn bij het ontwikkelen van Electron applicaties. Dit zijn simpele technieken zoals kijken wat de status is van het netwerk, heeft de computer een internetverbinding of niet. Dit zijn wel handige dingen die je applicatie helemaal compleet kunnen maken. 

Dit was de laatste theoretische sectie van de cursus, want in de volgende sectie wordt er een kleine applicatie gebouwd met het Electron framework. De lector heeft alle kenmerken van Electron goed uitgelegd. Dit framework biedt echt heel veel mogelijkheden om top desktopapplicaties te bouwen en dit zonder C# of Java dat we in de opleiding gezien hebben. 

## Sectie 8: Project
Dit is de laatste sectie van de cursus en hier wordt alle leerstof van de vorige secties samengevoegd door een applicatie te schrijven. Dit is een redelijk simpele applicatie dat je toelaat om websites toe te voegen die je later terug wilt lezen. Als je deze dan gelezen hebt via de applicatie kan je deze ook uit de lijst verwijderen. Via onderstaande link kan je de applicatie in actie zien.

<iframe width="100%" height="500" src="https://www.youtube.com/embed/zZTK8jCwY5Q?rel=0" frameborder="0" allowfullscreen></iframe>

Wanneer er een site wordt toegevoegd, dan wordt deze site in de achtergrond in een onzichtbaar browser venster geladen. Wanneer de site is ingeladen wordt er een screenshot genomen en word de titel van de site bewaard. Deze screenshot en titel worden gebruikt om de site in de lijst te tonen en het wordt ook bewaard op de computer, zodat je lijst niet verdwijnt als je de applicatie opnieuw opstart.

Voor de ontwikkeling van deze applicatie heb ik ook een GitHub repository gemaakt en per functionaliteit heb ik een commit gemaakt. De repository kan je terugvinden via de volgende link:

<a href="https://github.com/KoenCa/bookmarking-app " target="_blank">Repository</a>

Op het einde van deze sectie liet de lector ook zien hoe je deze applicatie kan compilen tot een applicatie voor Windows, Linux of Mac. 

## Reflectie
Deze cursus is een kort en bondige introductie tot het Electron framework. Ik heb geleerd hoe je HTML, CSS en JavaScript kan gebruiken om native desktopapplicaties te ontwikkelen voor elk bekend platform. In de opleiding hebben we geleerd hoe we dit met C# en Java kunnen doen. Nu dat ik ervaring heb opgedaan met Electron, denk ik dat ik zelf toch liever desktopapplicaties zou ontwikkelen met Electron. Je kan gebruik maken van veel bekende CSS frameworks voor de opmaak van je applicatie en voor de logica kan je gebruik maken van veel bekende JavaScript frameworks. Op deze manier hoef je als web developer niet een andere programmeertaal en manier van werken aan te leren om desktopapplicaties te ontwikkelen.

In het algemeen ben ik wel tevreden van deze cursus. De video’s zijn van hoge kwaliteit en je merkt dat de lector veel ervaring heeft met webdeveloping en Electron. Alles wat hij doet wordt ook duidelijk uitgelegd en hij schrijft ook veel commentaar in zijn code. Soms ging de lector wel snel waardoor ik de video op pauze moest zetten of moest terugspoelen, maar voor de rest heb ik er niet echt iets op aan te merken. 
