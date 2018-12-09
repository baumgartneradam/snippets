---
layout: default
codename: AlkFejlHf31
title: Határozott határozatlanság csapat tanulságai
tags: alkfejl
authors: Zolnai László, Schöberl Krisztián, Baumgartner Ádám
---

# Határozott határozatlanság csapat összefoglalója

## 1) Nem jelennek meg a változások?
Ha nem akarnak megjelenni a változások újrabuildelés során, megéri kitörölni a build könyvtárat.

## 2) QML debuggolása
QML debugoláshoz hasznos a QDebug << “” parancs, amivel a konzolban tudunk megjeleníteni üzeneteket.

## 3) Qt saját típusai
Néha váratlanul meg tudnak viccelni a Qt saját típusai, amiket ráadásul sok esetben nehéz debugolni. Pl. volt olyan függvény, ami hibátlanul működött QList<double>-lel és QList<int>-tel, de QList<float>-tal nem. 

## 4) Objektumok forgatása
Körülményes nem szimmetrikus objektumokat forgatni, célszerű ilyeneket választani.

## 5) Esztétikai tanácsok
### 5.1)
A legtöbb QT-ben fejlesztett alkalmazásnak nincs ikonja, ami nem kölcsönöz túl jó megjelenést. Az ikon hozzáadásához szükségünk van egy .ico fájlra a projektkönyvtárban, valamint az alábbi sort kell hozzáadni a projektfájlunkhoz: 
```RC_ICONS = robo.ico```

Ez után csak egy qmake választ el a profibb megjelenéstől minket.

### 5.2)
Érdemes pontosan vágni Photoshopban a képeket, különben ugrálni fog ha köztük váltunk.



