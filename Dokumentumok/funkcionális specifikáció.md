# Funkcionális specifikáció
## 1. Jelenlegi helyzet leírása  
A jelenlegi hírkeresési folyamatok fragmentáltak, sok forrás közül kell válogatni, melyek közül sok nem tekinthető megbízhatónak vagy részletesnek. A nagy médiafelületek gyakran elfogultak, és a felhasználói interakció nem mindig megfelelően moderált. A közösségi médián keresztüli informálódás nem kínál mély elemzéseket, és az algoritmusok befolyásolják a látható híreket. A felhasználók egy megbízható, központosított és interaktív hírportált keresnek, amely kiváló felhasználói élményt nyújt.
## 2. Vágyállomrendszer leírása
Egy web alapú alkalmazás létrehozása, ahol a felhasználók képesek híreket böngészni, olvasni és azokhoz kapcsolódó kommenteket megtekinteni. Az alkalmazás célja, hogy a látogatók gyorsan és egyszerűen tájékozódhassanak a legfrissebb eseményekről.  
Az alkalmazás adminisztrátorai képesek a hírek publikálására és a kommentek moderálására. Amennyiben egy komment vulgáris kifejezést, hamis információt vagy egyéb nem megengedett tartalmat tartalmaz, az adminisztrátoroknak lehetőségük van a komment törlésére, de annak szerkesztésére nincs lehetőség.  
A hírek és kommentek publikusan megtekinthetők minden látogató számára. Minden hírnek megjelenik a címe, egy rövid leírása, a publikálás dátuma és a hírt író szerző neve. A hírek alatt pedig helyet kapnak a hozzájuk tartozó kommentek, amelyek a közösségi interakciót és véleménynyilvánítást támogatják az adott hírekkel kapcsolatban.
## 3. Jelenlegi üzleti folyamatok modellje
 - 3.1. Hírek Kezelése
     - Felhasználók böngészhetnek és keresgélhetnek hírekhez.
 - 3.2. Felhasználói Interakció és Moderáció
     - Felhasználók megoszthatják véleményüket a hírek alatt.
     - Adminok ellenőrzik és kezelik a felhasználói hozzászólásokat.
 - 3.3. Felhasználói Felület és Regisztráció
     - Felhasználók regisztrálhatnak és bejelentkezhetnek.
     - Felhasználói felület lehetővé teszi a hírek böngészését és a vélemények megosztását.
 - 3.4. Tartalomkezelés és Adatbázis
     - Hatékony tartalomkezelési rendszerrel és adatbázissal rendelkezik az új hírek és cikkek kezeléséhez.
 - 3.5. Biztonság és Hibakezelés
     - Megfelelő biztonsági intézkedéseket alkalmaz az adatok védelme érdekében.
     - Hibakezelési mechanizmusokat tartalmaz a problémák kezeléséhez.
 - 3.6. Teljesítmény és Skálázhatóság
     - Jó teljesítményt nyújt, és skálázható a növekvő felhasználói forgalomhoz.
 - 3.7. Riportolás és Elemzés
     - Riportolási és elemzési eszközökkel rendelkezik az üzleti folyamatok figyelemmel kíséréséhez és értékeléséhez.

## 4. Igényelt üzleti folyamatok modellje
 - 4.1. Hírek Gyűjtése és Közzététele
     - Funkció: Hírek gyűjtése és közzététele a felhasználók számára.
     - Felelős: Adminok
     - Adminok híreket gyűjtenek különböző forrásokból, majd szerkesztik és formázzák azokat a weboldalon való közzététel céljából. Az alkalmazás automatikusan frissíti a híreket a különböző forrásokból.
 - 4.2. Felhasználói Interakció és Közösség
     - Funkció: Felhasználói vélemények megosztása és moderáció.
     - Felelős: Felhasználók, Adminok
     - A felhasználók lehetőséget kapnak a hírek alatti hozzászólások írására és véleményük megosztására. A adminok felelősek a hozzászólások azonnali ellenőrzéséért és moderálásáért annak érdekében, hogy biztosítsák a tartalom minőségét és a szabályszegések elkerülését.
 - 4.3. Mélyebb Elemzések és Cikkek
     - Funkció: Mélyebb elemzések és cikkek készítése.
     - Felelős: Admin     
 - 4.4. Felhasználói Felület és Testreszabhatóság
     - Funkció: Testreszabható felhasználói felület és preferenciák.
     - Felelős: Felhasználók
     - A felhasználók testreszabhatják a felületet az egyéni preferenciáiknak megfelelően. Választhatnak kedvenc témákat, beállíthatnak értesítéseket és követhetnek szerzőket a személyre szabott felhasználói élmény érdekében.
 - 4.5. Tartalom Minőségellenőrzés és Hibakezelés
     - Funkció: Tartalom minőségellenőrzés és hibakezelés.
     - Felelős: Adminok
     - Adminok folyamatosan ellenőrzik a tartalmat a szabályoknak megfelelően.
 - 4.6. Adatgyűjtés és Felhasználói Visszajelzés
     - Funkció: Adatgyűjtés és felhasználói visszajelzés elemzése.
     - Felelős: Felhasználók
     - Az alkalmazás gyűjti az adatokat a felhasználók viselkedéséről és visszajelzéseiről.
 - 4.7. Személyre Szabott Tartalom Ajánlások
     - Funkció: Személyre szabott tartalomajánlások.
     - Felelős: Algoritmusok
     - Az alkalmazás személyre szabott tartalomajánlásokat nyújt a felhasználóknak az alapján, hogy milyen híreket olvastak korábban és milyen témák érdeklik őket.

## 5. Követelménylista

| Id | Modul | Név | Leírás |
| --- | --- | --- | --- |
| FK1 | Felület | Comment | A felhasználók megtudják osztani gondoltaikat egy cikk vagy poszt alatt.|
| FK2 | Jogosultság| Bejelentkezési felület|A felhasználó az email címe és a jelszava segítségével bejelentkezhet. Az adatbázisban eltárolt jelszóval és felhasználónével ellentétben rossz adatérkezik a rendszer tájékoztat a sikertelen bejelntkezésről. |
| FK3 | Jogosultság | Regisztráció |A felhasználó a felhasználói nevének, email címének és jelszavának megadásával regisztrálja magát.Ha hibás adatokat visszbe arról a rendszer tajákoztatást ad egy hibaüzenet képében.|
| FK4 | Jogosultság| Jogosultsági szintek| -Admin:Rendszerhozzáférés, hírek feltöltése, felhasználók / szerepkörök módósítása. <br> -Felhasználó: Cikkek böngészése kommentelés.|
| FK5 | Modifikáció | Jelszó modosítás | A felhasználó módosítani tudja saját jelszavát.|
| FK6 | Modifikáció | Cikk törlése | Cikk törlése.|
| FK7 | Modifikáció | Cikk szerkesztése | Cikk szerkesztése.|
| FK8 | Modifikáció | Cikk létrehozása | Cikk írása,létrehozása,formázása.|

## 6. Használati esetek
**Felhasználó:**
- Hírfolyam böngészése: A felhasználó bejelentkezik egy közösségi média platformra, és böngészi a hírfolyamot, lájkolja vagy megosztja a bejegyzéseket, vagy kommenteket ír.
- Regisztráció és bejelentkezés: Egy felhasználó regisztrál egy weboldalon vagy alkalmazásban, majd bejelentkezik a fiókjába, hogy hozzáférjen a személyes adataihoz és funkciókhoz.
- Profilkezelés: A felhasználó szerkeszti a saját profilját, hozzáadja vagy módosítja a profilképét, frissíti az elérhetőségi adatait, vagy módosítja a jelszavát.

**ADMIN:** 
- Felhasználók kezelése: Az adminisztrátorok felügyelik és kezelik a felhasználói fiókokat, beleértve az új fiókok létrehozását, meglévők frissítését vagy deaktiválását.
- Hibaelhárítás és támogatás: Az adminisztrátorok segítenek a felhasználóknak, ha technikai problémáik vagy kérdéseik vannak, és hibaelhárítást végeznek, hogy megoldják a rendszerrel kapcsolatos problémákat.
- Biztonsági intézkedések: Az adminisztrátorok felelnek a rendszerbiztonságért, beleértve a felhasználók adatainak védelmét és az esetleges kiberbiztonsági fenyegetések elleni védelmet.
- Frissítések és karbantartás: Az adminisztrátorok frissítik az alkalmazást vagy a rendszert, hogy biztosítsák a funkciók és a biztonság folyamatos fejlesztését, valamint karbantartási tevékenységeket végeznek.
- Felhasználói jogosultságok kezelése: Az adminisztrátorok beállítják és ellenőrzik a felhasználói jogosultságokat, hogy biztosítsák, hogy minden felhasználó csak a megfelelő adatokhoz és funkciókhoz férhessen hozzá.
- Riportok és analitika: Az adminisztrátorok különböző riportokat és analitikai adatokat generálnak a rendszer teljesítményéről, amelyek segítenek az üzleti döntések meghozatalában.
- Adatbázis-kezelés: Az adminisztrátorok feladata lehet az adatbázisok kezelése, tartalmuk biztonságának és integritásának fenntartása.
- Tartalomkezelés: Az adminisztrátorok felelősek lehetnek a tartalom feltöltéséért, szerkesztéséért és eltávolításáért, például blogbejegyzések, cikkek vagy képek esetén.

## 7. Megfeleltetés, hogyan fedik le a használati eseteket a követelményeket
| Lefedett használati eset | Követelmény | Követelmény azonosító(k) |
| --- | :--: | :--: |
| A felhasználó az email címe és a jelszava segítségével bejelentkezhet. Az adatbázisban eltárolt jelszóval és felhasználónével ellentétben rossz adatérkezik a rendszer tájékoztat a sikertelen bejelntkezésről. | Bejelentkezési felület | K2 |
| A felhasználó a felhasználói nevének, email címének és jelszavának megadásával regisztrálja magát. Ha hibás adatokat visszbe arról a rendszer tajákoztatást ad egy hibaüzenet képében. | Regisztrációs felület | K3 |
| A felhasznákóknak megjelennek a hírek és megtudják osztani gondoltaikat egy cikk vagy poszt alatt és híreket tudnak böngészni. | Felület | K1, K4 |
| A felhasználók a felhasználói adatoknál jelszavat tud változtatni. | Jelszó módosítás | K5 |
| Admin felhasználó cikkeket hozhat létre, cikkeket törölhet és szerkeszthet. | Admin jogosultság | K6, K7, K8 |

## 8. Képernyőtervek

![lgnrgst](../Képernyőtervek/loginregister.PNG)
![fooldal](../Képernyőtervek/fooldal.PNG)

## 9. Forgatókönyvek
A felhasználók a weboldalon böngészik a legfrissebb híreket és olvashatnak. Az adminisztrátorok felügyelik a tartalom minőségét.

1. Bejelentkezés
 - A felhasználó megadja a felhasználónevét és jelszavát.
 - Sikeres bejelentkezés esetén megjelenik a hírportál kezdőlapja.
 - Sikertelen bejelentkezés esetén értesítést kap és visszalép a Bejelentkező felületre.

2. Regisztráció
 - A felhasználó megadja regisztálni kívánt a felhasználónevét, e-mail címét, jelszavát és jelszó ismétlését.
 - Sikeres regisztráció esetén értesítést kap és a bejelentkező felületre lép.
 - Sikertelen regisztráció esetén értesítést kap a hibáról és visszalép a regisztrációs felületre.

3. Kezdőlap
 - A felhasználók híreket böngésznek és kommentelhetnek alatta.
 - Az admin felhasználók szerkessztheti a meglévő híreket, törölhetnek híreket és létrehozhatnak új híreket.

4. Felhasználói adatok
 - A felhasználók megtekinthetik a saját felhasználói adataikat és jelszavat módosíthatnak.
 - Az admin felhasználók módosíthatják a felhasználói jogosultságokat és a felhasználókat moderálhatják (kitilthatják).

## 10. Funkció - követelmény megfeleltetése

| Id | Követelmény | Funkció | 
| -- | -- |---| 
| K1 | FK3 | M3 |  
| K2 | FK2 | M2 |  
| K3 | FK4 | M4 |  
| K4 | FK1 | M1 |  
| K5 | FK6, FK7, FK8 | M6, M7, M8 |  

## 11 Fogalomszótár

- **Web alapú alkalmazás:** - A Web alapú kezelés egy olyan segédprogram, amely egy szokványos webböngészőt használ a készülék HTTP és HTTPS protokollal történő kezeléséhez.
- **Adatbázis:** - Az adatbázis (DB: Database) számítógépen (általában háttértárakon) tárolt adatok összessége.

[def]: fooldal.PNG