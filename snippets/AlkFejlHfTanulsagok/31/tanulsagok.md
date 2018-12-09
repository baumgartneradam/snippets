---
layout: default
codename: AlkFejlHf31
title: Határozott határozatlanság csapat tanulságai
tags: alkfejl
authors: Zolnai László, Schöberl Krisztián, Baumgartner Ádám
---

# Határozott határozatlanság csapat összefoglalója

## 1) 
Ha nem akarnak megjelenni a változások újrabuildelés során, megéri kitörölni a build könyvtárat.

## 2) Objektumok forgatása
Körülményes nem szimmetrikus objektumokat forgatni, célszerű ilyeneket választani.

## 3) QML debuggolása
QML debugoláshoz hasznos a QDebug << “” parancs, amivel a konzolban tudunk megjeleníteni üzeneteket.

## 4) Esztétikai tanácsok
### 4.1)
A legtöbb QT-ben fejlesztett alkalmazásnak nincs ikonja, ami nem kölcsönöz túl jó megjelenést a fejlesztésünknek. 
Az ikon hozzáadásához szükségünk van egy .ico filera a projektkönyvtárban, valamint az alábbi sort kell hozzáadni a projektfileunkhoz:
RC_ICONS = robo.ico
Ez után csak egy qmake választ el a profibb megjelenéstől minket.

### 4.2)
Érdemes pontosan vágni Photoshopban a képeket, különben ugrálni fog ha köztük váltunk.



