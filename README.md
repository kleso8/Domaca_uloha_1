DOMÁCA ÚLOHA 1 - ZOBRAZENIE

Zadanie:

Pre zvolené zobrazenie (Marinovo, Lambertovo, Braunovo a Mercatorovo) a mierku vypísať
súradnice rovnobežiek a poludníkov. Súradnice po 10°, polomer Zeme 6371,11 km. Výstupom 
zoznam vzdialeností súradníc od stredu papiera. Vzdialenosti v centimetroch s presnosťou
na milimetre. Ak vzdialenosť prekročí 1 meter, vypíše sa namiesto čísla pomlčka.

Vstupy programu:

Program obsahuje interaktívne vstupy. Najprv sa užívateľa spýta na to, aké chce počítať
zobrazenie. Zadať musí jedno z týchto písmen: L pre Lambertovo zobrazenie
                                              A pre Marinovo zobrazenie
                                              B pre Braunovo zobrazenie
                                              M pre Mercatorovo zobrazenie
Program funguje len pre tieto 4 zobrazenia. Ak užívateľ nezadá žiadne alebo iné písmeno,
program skončí a informuje užívateľa, že zadal nesprávne písmeno. Naopak, ak 
užívateľ zadá jedno z týchto 4 písmen, tak program sa ho spýta na mierku mapy. Program 
bude ďalej pracovať len v prípade, že užívateľ zadá kladnú hodnotu celého čísla. Ak 
zadá nulu, záporné číslo alebo necelé číslo, tak program skončí a informuje užívateľa, 
že zadal nesprávnu mierku mapy. Po zadaní správnej hodnoty sa program spýta na polomer
Zeme. Tu ponúka užívateľovi zadať vlastnú hodnotu polomeru alebo zadať nulu. Po zadaní 
nuly bude program počítať s polomerom 6371,11 km. Ak užívateľ zadá zápornú hodnotu
polomeru, tak program skončí a informuje užívateľa o tom, že zadal záporný polomer Zeme. 

Funkcie programu:

Po splnení všetkých podmienok vstupov bude program pokračovať ďalej. Najprv sa prepočíta 
užívateľom zadaný polomer Zeme na centimetre a predelí sa užívateľom zadanou mierkou mapy.
Vznikne tak nová premmenná, ktorá sa použije vo vzorcoch daných výpočtov.

Ako prvé počíta program poludníky. Vytvorí sa prázdny zoznam a cyklus, v ktorom sa 
zadávajú hodnoty daných poludníkov po 10° od -180° po 180°. Cez vzorec výpočtu 
poludníkov, ktorý je pre všetky zobrazenia rovnaký, sa vypočítajú hodnoty x, 
ktoré reprezentujú zvislú vzdialenosť poludníkov na paprieri od stredu papiera.
Tieto hodnoty sa priradia do zoznamu a zaokrúhlia sa na jedno desatinné miesto. 
Hodnoty v zozname nad 1 meter program zmení na pomlčku.

Následne program počíta rovnobežky. Opäť vytvorí prázdny zoznam a cyklus. Tu sa zadajú 
hodnoty rovnobežiek po 10° od -90° po 90°. Tento cyklus program počíta pre Lambertovo,
Marinovo a Braunovo zobrazenie. Cez vzorce daných zobrazení sa vypočítajú hodnoty y, 
ktoré reprezentujú vodorovnú vzdialenosť poludníkov na paprieri od stredu papiera. 
Hodnoty sa priradia do zoznamu rovnobežiek.

Pre Mercatorovo zobrazenie program vytvorí vlastný cyklus. Je to z toho dôvodu, že 
hodnoty pre 90° a -90° vzorec pre výpočet rovnobežiek nedokáže vypočítať, keďže tam 
dochádza k deleniu nulou. Preto je cyklus obmedzený na -80° až 80°. Opäť sa tu 
vypočítajú hodnoty y ako u ostatných zobrazení a hodnoty sa priradia do zoznamu 
rovnobežiek. K tomuto zoznamu program priradí aj jednu hodnotu na začiatok a jednu na 
koniec zoznamu, a tie reprezentujú práve hodnoty 90° a -90°, ktoré smerujú do nekonečna.

Hodnoty rovnobežiek v zozname sa zaokrúhlia na jedno desatinné miesto a zoradia sa od
najmenšieho čísla po najväčšie. Hodnoty v zozname nad 1 meter program zmení na pomlčku.

Výstupy programu:

Výstupom programu sú zoznamy poludníkov a rovnobežiek. Tie reprezentujú vzdialenosti 
daných súradníc od stredu papiera, pričom nula reprezentuje práve tento stred. Tieto 
vzdialenosti sú v centimetroch a zaokrúhlené na milimetre. Po nanášaní týchto 
vzdialeností na papier je užívateľ schopný nakresliť požadadované zobrazenie rýchlo 
a efektívne.
