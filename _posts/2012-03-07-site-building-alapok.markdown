
---
layout: post
title:  01. Site building alapok
---

A Drupal site building alapok átismétléséhez a következő forrásokat ajánlom.
Ezek többnyire a hivatalos Drupal dokumentáció részei, és jóval részletesebbek
mint az órán vett anyag.

## Drupal telepítése

- [Installation Guide][dinst] - Hivatalos Drupal dokumentáció
- [Drupal 7 telepítése][hd7inst] - Magyar Drupal kézikönyv
- [Drupal telepítése lépésről lépésre][hdinst] - Magyar Drupal kézikönyv _(ez
  egy korábbi Drupal verzióval mutatja be, de részletesebb az adatbázis
  előkészítése szempontjából)_

## Alapvető adminisztrációs műveletek

- [Getting started with Drupal 7 administration][dadmin]
- [Creating content][ccont]

## Views

A Views kezeléséhez talán legjobb a NodeOne video-tutorial sorozata: [Taming the
Beast: Learn Views with NodeOne][noviews], az 1-7. rész az, amiket az órán is
kipróbáltunk, de nyugodtan tovább is lehet menni.

## Híroldal felépítésének lépései
_(amit az órán sikerült összehozni)_

1.  Új szótár létrehozása a rovatoknak
2.  Szótár hozzáadása (field-ként) az Article tartalomtípushoz
3.  Tartalom generálása Devel generate modullal
4.  Blokk nézet létrehozása a rovatoknak
5.  Blokkok elhelyezése
6.  Kép mező átalakítása, hogy több képet is feltölthessünk
7.  Colorbox modul telepítése
8.  Article tartalomtípusban a megjelenés átállítása Colorbox slideshow-ra
9.  Views slideshow telepítése
10. Nézet létrehozása a kiemelt tartalmaknak, views slideshow megjelenítéssel

## Használt modulok

- [Drupal 7][d7core] (alaprendszer moduljait nem sorolom fel...)
- [Views][views]
- [Chaos Tool Suite][ctools] (Views függősége)
- [Devel][devel]
- [Views slideshow][vsl]
- [Colorbox][colorbox]

## [Drush][drush] parancsok

- Drush help

        drush help
        drush help pml

- Modulok listázása: `pm-list` vagy `pml`

        drush pml
- Modulok letöltése: `pm-download` vagy `dl`

        drush dl views ctools
- Modulok telepítése: `pm-enable` vagy `en` (`-y` hogy ne kérdezzen)

        drush en -y views_ui
- Modulok kikapcsolása: `pm-disable` vagy `dis`

        drush dis -y color

## További hasznos parancsok

Például a külső JS library-k telepítéséhez:

- `wget http://example.com` - fájl letöltéséhez
- `unzip filename.zip` - zip fájl kicsomagolásához



[dinst]: http://drupal.org/documentation/install
[hd7inst]: http://drupal.hu/kezikonyv/drupal7-telepites
[hdinst]: http://drupal.hu/kezikonyv/telepites
[dadmin]: http://drupal.org/getting-started/7/admin
[ccont]: http://drupal.org/node/120635
[noviews]: http://dev.nodeone.se/en/taming-the-beast-learn-views-with-nodeone
[d7core]: http://drupal.org/project/drupal
[views]: http://drupal.org/project/views
[ctools]: http://drupal.org/project/ctools
[devel]: http://drupal.org/project/devel
[vsl]: http://drupal.org/project/views_slideshow
[colorbox]: http://drupal.org/project/colorbox
[drush]: http://drupal.org/project/drush
