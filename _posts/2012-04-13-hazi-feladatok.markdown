---
layout: post
title: Házi feladatok
---

A [házi feladatokat][hf] a github issue tracker-ében teszem közzé, és minden
kérdést és hozzászólást ami a feladatokhoz kapcsolódik ott kell feltenni, és ott
is adok választ.

## Github

Ezért először is mindenkinek szüksége lesz egy github account-ra.
<https://github.com/signup/free>

Ez a lista folyamatosan bővülni fog. A feladatok többsége nem túlságosan nehéz,
ezért többet is meg lehet/kell oldani.

## Csapatmunka OK, egy feladatra csak egy megoldás!

Egy feladatra egyetlen megoldást fogadok el. Ez azt jelenti, hogy két ember NE
oldjon meg egy feladatot egymástól függetlenül!

Összedolgozni, egymásnak segíteni azonban lehet, sőt: az volna az igazán jó, ha
többen is hozzászólnának, kérdeznének egy feladattal kapcsolatban. Mindez a
feladathoz tartozó issue oldalon történjen, így láthatom mindenki aktivitását.

Az sem probléma, ha egy feladat kódolásában is többen vesznek részt, ez azonban
nehezen kivitelezhető a Git és a github ismerete nélkül.

## Határidők (milestones)

Néhány feladat [határidőhöz][ms] van/lesz kötve. Ezek a határidők mindig az óra
előtti napok (tehát szerdák). Ezek olyan feladatok, melyeket mindenképpen meg
kell oldani ahhoz, hogy a következő órán tovább haladhassunk az anyaggal,
ugyanakkor nem akarok ezek miatt az órából időt elvenni, mert semmi új és extra
nincs a megoldásban.

A határidős feladatok prioritást élveznek, bőkezűbben osztogatom majd a pontokat
a résztvevőknek. (És még kitalálok valami negatív következményt is arra az
esetre, ha senki nem akarna foglalkozni ezekkel a feladatokkal...)

_A következő óráig (ápr 19.) egyébként [2 feltétlenül megoldandó feladat][0418]
van._

## Nem csak a kód!

Egy feladat megoldása nem feltétlenül csak a kód elkészítéséből áll. A
feladatkiírásokon is látszik, hogy nincs minden feladat alaposan megfogalmazva,
és kitalálva. Többnyire csak a probléma rövid leírása szerepel, tehát a legtöbb
esetben az is a feladat része, hogy kitaláljuk, hogy mi a feladat.

Tehát **nem a kód a lényeg,** hanem **a problémamegoldás.**

Azaz, ha valamit nem értesz tisztán, nem vagy teljesen biztos, akkor kérdezz,
írd le a saját elképzelésedet, mert az még mindig kevesebb munka, mint olyasmin
dolgozni, amire nincs is szükség. Mindezt az issue oldalán hozzászólásban
_(email-ben nem fogok válaszolni)_, hogy mindenki más is láthassa, és könnyebben
megérthesse a problémát.

A kérdésekre bárki válaszolhat! Sőt, valószínűleg több esetben várni is fogok a
válasszal, hogy más is hozzászólhasson a témához.

## Új issue-t bárki írhat

Új issue-t, vagyis feladatot bárki megfogalmazhat. Ha találsz egy hibát, vagy
van egy ötleted újabb funkcióra, nyugodtan készíts új issue-t, és az arra kapott
reakciókból kiderül, hogy érdemes-e megvalósítani, vagy sem.

## Coding standards

Csak olyan megoldást fogadok el, ami megfelel a [Drupal coding
standards][cs]-nek.

A [Coder][coder] modul hasznos lehet mindenkinek!

## A javasolt munkamenet

A Git és a github nagyon jó eszköz arra, hogy ezeket a feladatokat könnyen
tudjuk kezelni, ehhez azonban kicsit alaposabban kell ismerni a rendszert. Ezt
sajnos nem tudom most megkövetelni, de leírom az általam favorizált megoldást,
nem olyan bonyolult, próbálkozni kell:

1. A megoldáshoz [fork][fork]-olni kell az eredeti repository-t, és ezt kell
   módosítani.
2. Ha a megoldást megfelelőnek érzed, küldeni kell egy [pull request][pr]-et,
   hogy mások is megnézhessék, és ha valóban jó a megoldás, akkor be fogom
   emelni a kódba a módosításokat.

Azért ez a favorizált megoldási forma, mert így a módosítások mindenki számára
láthatóak lesznek a githubon, és könnyen kezelhetőek.

Ehhez minden eszköz rendelkezésre áll a szerveren.

## A nem javasolt munkamenet...

A fent említett folyamat nem is olyan bonyolult mint amilyennek az angol
kifejezések láttatják, de nem várom el, hogy mindenki elsőre adaptálja, a lényeg
mégiscsak az, hogy haladjon a munka, így van egy egyszerűbbnek tűnő módszer is:

1. Ezt mindenképpen a szerveren kell megcsinálni, akár egy friss Drupal
   telepítéssel.
2. A változtatásoknak mindig a githubon aktuálisan közzétett kódbázison kell
   történni, tehát kell egy másolat róla. Ez megoldható
     - a repository [klónozásával][clone]/[frissítésével][pull],
     - vagy a zippelt kód letöltésével ([ott a zip gomb a fejlécben][ghmb])
3. Ha a megoldást megfelelőnek érzed, jelzed az issue oldalán, hogy a szerveren.
   hol tudom leellenőrizni, és én majd készítek belőle egy pull request-et.

Azét legalább egyszer mindenki próbálja meg a favorizált módszert...

Természetesen szívesen válaszolok a fent leírtakkal kapcsolatban felmerült
kérdésekre.

[hf]: https://github.com/dCourse/shrtr/issues?milestone=&sort=created&direction=desc&state=open
[ms]: https://github.com/dCourse/shrtr/issues/milestones
[0418]: https://github.com/dCourse/shrtr/issues?milestone=1&state=open
[ghmb]: https://github.com/dCourse/shrtr
[clone]: http://gitref.org/creating/#clone
[pull]: http://gitref.org/remotes/#fetch
[fork]: http://help.github.com/fork-a-repo/
[pr]: http://help.github.com/send-pull-requests/
[cs]: http://drupal.org/coding-standards
[coder]: http://drupal.org/project/coder
