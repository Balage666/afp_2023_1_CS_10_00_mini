# Követelmény specifikáció

## 1. Áttekintés
A tájékozódás és informálódás napjainkban egyre inkább az online térbe költözik, és egyre többen keresik a friss híreket és információkat online forrásokból. Ennek megfelelően egy olyan hírportál létrehozása a cél, amely aktuális, releváns és megbízható hírekkel szolgál a felhasználók számára. A portál egy központi platformot kínál a legfrissebb hazai és nemzetközi hírekkel, eseményekkel, véleményekkel és elemzésekkel, valamint egy olyan közösségi platformot is biztosít, ahol a felhasználók hozzászólhatnak és megoszthatják véleményüket.

## 2. A jelenlegi helyzet leírása  
A hírek és információk keresésének folyamata jelenleg fragmentált. Számos hírforrás, blog és weboldal kínálja saját tartalmát, de nincs olyan központosított platform, amely átfogó képet adna a legfontosabb hírekről és eseményekről. Bár néhány nagyobb hírportál és médiafelület létezik, sokan azokat politikailag elfogultnak vagy nem eléggé részletesnek tartják. Emellett a hozzászólások és a felhasználói interakció gyakran korlátozott vagy nem megfelelően moderált, ami negatívan befolyásolhatja a közösségi élményt és a felhasználói megbízhatóságot.
Sokan a közösségi média oldalakon keresztül próbálnak informálódni, azonban ezek az oldalak gyakran nem kínálnak mélyebb elemzéseket vagy kontextust a hírekhez, valamint az algoritmusok befolyásolják azt, hogy milyen hírek jelennek meg a felhasználók előtt.  
A hírekhoz való könnyű és gyors hozzáférés mellett a felhasználók egyre nagyobb hangsúlyt fektetnek a megbízhatóságra és a tartalom hitelességére, amit jelenleg kevés platform tud teljes mértékben biztosítani.  
A cél tehát egy olyan hírportál létrehozása, amely ötvözi a megbízhatóságot, a központosított hírszolgáltatást és a felhasználói interakciót, miközben kiváló felhasználói élményt biztosít.

## 3. Vágyálomrendszer
 Nem csak egy passzív olvasói élményt nyújt. Szeretnénk, ha  a felhasználók aktívan részt vennének a hírek és információk terjesztésében és megvitatásában. Minden egyes látogató számít számunkra, és mi segítünk abban, hogy könnyen megossza véleményét és tapasztalatait.
 A hírportál célja, hogy hozzáférést biztosítson az információkhoz, hogy a felhasználók is hatékonyan formálhassa véleményét és döntéseit, továbbá  szeretnénk ha itt találnák meg a friss és releváns információkat minden olyan területen, ami fontos. Legyen az a legújabb helyi hír, a globális események, tudományos felfedezések, vagy éppen a legújabb technológiai újdonságok

## 4. Jelenlegi üzleti folyamatok modellje
 - 4.1. Hírek Gyűjtése és Közzététele
     - Felelős: Admin
     - Folyamat: Adminok gyűjtik és formázzák a híreket, majd közzéteszik azokat a weboldalon.
 - 4.2. Felhasználói Interakció és Közösség
     - Felelős: Felhasználók, Adminok
     - Folyamat: Felhasználók hozzászólnak és megosztják véleményüket, melyet adminok ellenőriznek.
 - 4.3. Mélyebb Elemzések
     - Felelős: Admin     

## 5. Igényelt üzleti folyamatok modellje
 - 5.1. Hírek Gyűjtése és Közzététele
     - Felelős: Admin
     - Folyamat: Adminok gyűjtik és formázzák a híreket, majd közzéteszik azokat a weboldalon. Emellett az alkalmazás automatikusan frissíti a híreket a különböző forrásokból.
 - 5.2. Felhasználói Interakció és Közösség
     - Felelős: Felhasználók, Adminok
     - Folyamat: Felhasználók hozzászólnak és megosztják véleményüket a hírek alatt. Adminok azonnal ellenőrzik és kezelik a hozzászólásokat, hogy biztosítsák a tartalom minőségét és a trollkodás vagy szabályszegések elkerülését.
 - 5.3. Mélyebb Elemzések és Cikkek
     - Felelős: Admin
 - 5.4. Felhasználói Felület és Testreszabhatóság
     - Felelős: Felhasználók
     - Folyamat: A felhasználók testreszabhatják a felületet, hogy az megfeleljen az egyéni preferenciáiknak, például választhatnak kedvenc témákat, beállíthatnak értesítéseket és következhetnek szerzőket.
 - 5.5. Tartalom Minőségellenőrzés és Hibakezelés
     - Felelős: Adminok
     - Folyamat: Adminok folyamatosan ellenőrzik a tartalmat a szabályoknak megfelelően.
 - 5.6. Adatgyűjtés és Felhasználói Visszajelzés
     - Felelős: Felhasználók, Adminok
     - Folyamat: Az alkalmazás gyűjti az adatokat a felhasználók viselkedéséről és visszajelzéseiről.
 - 5.7. Személyre Szabott Tartalom Ajánlások
     - Felelős: Algoritmusok
     - Folyamat: Az alkalmazás személyre szabott tartalomajánlásokat nyújt a felhasználóknak az alapján, hogy milyen híreket olvastak korábban és milyen témák érdeklik őket.

## 6. Követelménylista
| Id | Modul | Név | Leírás |
| --- | --- | --- | --- |
| M1 | Felület | Comment | A felhasználók megtudják osztani gondoltaikat egy cikk vagy poszt alatt.|
| M2 | Jogosultság| Bejelentkezési felület|A felhasználó az email címe és a jelszava segítségével bejelentkezhet.|
| M3 | Jogosultság | Regisztráció |A felhasználó a felhasználói nevének, email címének és jelszavának megadásával regisztrálja magát.|
| M4 | Jogosultság| Jogosultsági szintek| -Admin:Rendszerhozzáférés, hírek feltöltése, felhasználók / szerepkörök módósítása. <br>-Felhasználó: Cikkek böngészése, kommentelés.|
| M5 | Modifikáció | Jelszó modosítás | A felhasználó módosítani tudja saját jelszavát.|
| M6 | Modifikáció | Cikk törlése | Cikk törlése.|
| M7 | Modifikáció | Cikk szerkesztése | Cikk szerkesztése.|
| M8 | Modifikáció | Cikk létrehozása | Cikk írása,létrehozása,formázása.|

## 7. Fogalomtár
 - **Reszponzív felület** - Mobilon, Tableten, PC-n igazodik a
képernyőhöz a felület mérete, azaz több eszközön is probléma nélkül
üzemelhet.  
 - **Comment** - rövid írásos kifejezés, amelyet egy személy vagy több személy ír, mond vagy oszt meg egy online vagy offline közegben, hogy kifejezze véleményét, észrevételeit vagy gondolatait egy adott témával, cikkel, poszttal vagy eseménnyel kapcsolatban.
