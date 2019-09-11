# Setup guide SDL2 MS Visual Studio 
## Stap 1:
Download de latest development versie van SDL2 [hier](http://libsdl.org/download-2.0.php)

Extract de files naar de root van je C schijf **C:\sdl2**
## Stap 2:
Start een empty c++ project, of clone een bestaand c++ project van github
## Stap 3:
Selecteer je c++ project in Solution Explorer en druk op **Alt+Enter**

![](https://i.imgur.com/n0CO9du.png)

## Stap 4: 

![]https://i.imgur.com/mXb19x0.png)

Zorg ervoor dat de configuration op All configurations staat en dat het platform op Active(x64) staat.

## Stap 5:
_VC++ Directories > Include Directories > Edit_

![](https://i.gyazo.com/7e8bc9f7589bee8406efb2c9d85dd3e2.png)

Voeg het volgende path **C:\sdl2\include** toe. Nu weet Visual Studio waar alle SDL2 header files staan.

![](https://i.gyazo.com/0cd7912745a57471feca6eca48e73be8.png)

## Stap 6:
_VC++ Directories > Library Directories > Edit_

Voeg het volgende path **C:\sdl2\lib\x64** toe. Dit path verwijst naar de librairies van SDL2.

## Stap 7:
Nu gaan we de compiler linken met de librairies.
_Linker > Input > Additional Dependencies > Edit_

Voeg de vogende files toe:

* SDL2.lib;
* SDL2main.lib;

![](https://i.gyazo.com/2595677a9517153413bad82104370d2a.png)

## Stap 8:

Zet de subsystem op Console, nu is het mogelijk om debug messages over de console schrijven.

Wanneer dit niet meer nodig is wijzig het naar: Windows subsystem

![](https://i.gyazo.com/9788931b67d8126147714ae653e645c6.png)



