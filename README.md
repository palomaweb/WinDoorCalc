Elnézést a félreértésért! Itt van egy módosított változat, amely csak a README tartalmát tartalmazza, instrukciók nélkül, így egyből bemásolható lesz:

```
# Árajánlatkérő Webalkalmazás

Laravel alapú árajánlatkérő- és kezelő rendszer. Speciálisan ablakok, ajtók és kiegészítőik megvásárlásához, beszereléséhez kérhető ajánlat. Az árajánlatot a rendszer automatikusan generálja és elküldi az igénylő e-mail címére PDF formátumban.

## Funkciók

- Árajánlatok automatikus generálása.
- PDF formátumú árajánlat küldése e-mailben.
- Speciális igények szerinti testreszabás (ablakok, ajtók és kiegészítőik).
- Admin felület a beérkezett ajánlatok kezelésére.

## Telepítés

### 1. Clone-ozás

Először klónozd a projektet a saját gépedre:

```bash
git clone https://github.com/felhasznalo/ajanlatkeres.git
```

### 2. Composer telepítése

A projekt Composer-t igényel a függőségek kezelésére. Ha nincs telepítve, telepítsd a következő parancs segítségével:

```bash
composer install
```

### 3. Környezeti fájl beállítása

Hozd létre a `.env` fájlt a következő parancs használatával:

```bash
cp .env.example .env
```

Ezután generáld le az alkalmazás kulcsát:

```bash
php artisan key:generate
```

### 4. Adatbázis beállítás

Állítsd be az adatbázis kapcsolatot a `.env` fájlban a saját adatbázisodnak megfelelően.

### 5. Migrációk futtatása

Futtasd a migrációkat az adatbázis struktúrájának létrehozásához:

```bash
php artisan migrate
```

### 6. Fejlesztői szerver indítása

Indítsd el a beépített fejlesztői szervert:

```bash
php artisan serve
```

A szerver alapértelmezés szerint a `http://localhost:8000` címen lesz elérhető.

## Használat

1. Látogass el a webalkalmazás főoldalára.
2. Töltsd ki az ajánlatkérő űrlapot az ablakok, ajtók és egyéb termékek adataival.
3. Kattints az "Árajánlat kérése" gombra.
4. A rendszer automatikusan generálja az árajánlatot, amely PDF formátumban azonnal elküldésre kerül a megadott e-mail címre.

## Tesztelés

A projektben tesztelési szkriptek találhatóak, melyek futtatásához használd a következő parancsot:

```bash
php artisan test
```

Ez futtatja a teszteket, és ellenőrzi, hogy a rendszer megfelelően működik.

## License

This project is intended solely for viewing and demonstration purposes. 
You may not modify, distribute, or use this project for commercial purposes.