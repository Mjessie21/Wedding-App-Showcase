# EskuvoFoglalo - Esküvői Helyszínlefoglaló Mobilalkalmazás 💍

Az **EskuvoFoglalo** egy modern, Jetpack Compose alapú Android alkalmazás, amely a legújabb mobilfejlesztési irányelveket követve segíti a párokat az ideális esküvői helyszín megtalálásában és a kapcsolatfelvételben.

> **Fontos közlemény:** Az alkalmazás forráskódja az egyetemi szabályzat és az automatizált mérföldkő-ellenőrző rendszerek védelme érdekében nem publikus. Ezért ezzel a repository -val a projekt architektúráját, tervezési döntéseit és funkcionális felépítését szeretném bemutatni.

## Technológiai Stack & Architektúra
Az alkalmazás fejlesztése során a cél a **tiszta kód (Clean Code)** és a **moduláris felépítés** volt:
*   **Nyelv:** Kotlin
*   **UI Keretrendszer:** Jetpack Compose (Modern, deklaratív UI)
*   **Design System:** Egyedi Material 3 téma (WeddingTheme) pezsgő/arany és krém színekkel, elegáns Serif tipográfiával.
*   **Adatkezelés:** Firebase (Autentikáció és valós idejű adatbázis).
*   **Architektúra:** MVVM (Model-View-ViewModel) komponens-alapú szétválasztással (`ui.screens`, `ui.components`).

## Kiemelt Funkciók
*   **Dinamikus Helyszínadatlapok:** Kapacitás, árazás és szolgáltatások megjelenítése interaktív ikonokkal.
*   **Adaptív Megjelenítés:** Teljes körű támogatás álló és fekvő módhoz (Adaptive Grid), valamint különböző képernyőméretekhez.
*   **Intelligens Navigáció:** Állapotalapú navigációs gráf, amely kezeli a Welcome, Home és Detail szinteket.
*   **Akadálymentesség (Accessibility):** Teljes TalkBack támogatás dinamikus leírásokkal és szemantikai módosítókkal.

## Adatmodell és Logika
A rendszer komplex entitáskapcsolatokat kezel (Venue, Service, User, BookingRequest), biztosítva a skálázhatóságot:
*   **DAO-szerű megközelítés:** Az adathozzáférés elszigetelése a UI-tól.
*   **N:M kapcsolatok kezelése:** Helyszínek és szolgáltatások összekapcsolása.

## Képernyőképek
<p align="center">
  <img src="bejelentkezes.jpg" width="30%" title="Bejelentkezés" alt="Bejelentkezés" />
  <img src="fooldal.jpg" width="30%" title="Kezdőlap" alt="Kezdőlap" />
  <img src="helyszinek.jpg" width="30%" title="Helyszínek listája" alt="Helyszínek listája" />
</p>
<p align="center">
  <img src="adatlap.jpg" width="30%" title="Helyszín adatlapja" alt="Helyszín adatlapja" />
  <img src="datumvalaszto.jpg" width="30%" title="Dátum kiválasztása" alt="Dátum kiválasztása" />
  <img src="ajanlatkeres.jpg" width="30%" title="Ajánlatkérés véglegesítése" alt="Ajánlatkérés véglegesítése" />
</p>
<p align="center">
  <img src="ajanlataim.jpg" width="30%" title="Foglalások áttekintése" alt="Foglalások áttekintése" />
</p>

---
*Készítette: Makai Dzsesszika (Mjessie21)*
