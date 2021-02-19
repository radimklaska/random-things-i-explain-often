# Útržky

Pár témat a otázek na které odpovídám poměrně pravidelně. - Potřebuji místo kam mohu sypat náhodné útržky z konverzací. To bude tady.

Pokud Ti stránka ušetří trochu sepisování a vysvětlování, nebo Tě sem někdo poslal a informace Ti pomohly, zvaž kolik času to ušetřilo a koukni na [https://github.com/sponsors/radimklaska](https://github.com/sponsors/radimklaska) ;-) Díky. 

## Péče o Li-Pol baterie

TL;DR:
* označení zapojení: `4S2P`
  * počet článků sériově udáván jako "S" (více článků = větší celkové napětí)
  * počet článků paralelně udáván jako "P" (více článků = vštsí kapacita a max proud)
  * zjednodušeně: `4S`, zde se předpokládá a nepíše `1P`
* 3,8V až 4,2V na každý článek.
* Nikdy nevybíjet pod cca 3,4V (rychlá degradace)
* Při zátěži vybít max cca do 3,6V.
  * Po odpojení by se baterka měla sama stabilizovat zpět kolem 3.8V
* Baterie skladovat na s napětím 3,8V na článek

Li-Polky by se vždy měly nabíjet s balancováním (ballance charge). Některé nabíječky umí rychlé nabíjení bez "jemného" balancování na konci (fast charge). Bez balančního konektoru bych nabíjet nedoporučoval.

Li-Pol nemají paměťový efekt - nepotřebují kompletní cyklus nabití "z nuly na sto procent a vybít zpět do nuly".

Pokud se delší dobu nebudou používat (řekněme cca 4 dny a více) tak je potřeba je vybít na skladovací napětí (storage charge). To je 3,8V na každém článku. Při takovém napětí by mělo být možné baterku skladovat teoreticky i pár let. Ale je dobré je jednou za čas kontrolovat jestli nějaký článek "neujíždí". Kontroloval bych z počátku cca 1x za měsíc. Když se napětí drží blízko 3,8V, tak klidně i méně často.

Pokud baterku necháte plně nabitou delší dobu, tak bude při zátěži rychle ztrácet napětí. Často se to i projeví tím že se fyzicky nafoukne.

A poslední pravidlo je baterku nepodvybít. Při zátěži může napětí článků klesnout az cca k 3,5V. Po vyndání z auta by se měla po cca deseti minutách zase stabilizovat kolem 3,8V na článek. Vybití pod cca 3,3V na článek už znamená prakticky okamžitou degragaci baterie. Ne že by nutně byla hned nepoužitelná, ale takovou baterii bych si označil a věnoval větší pozornost vybalancování a kapacitě, teplotě při zátěži.

V příslušenství máte připravený měřák. Po připojení na balanční konektor ukáže celkové napětí a pak napětí na každém článku. Umí i varovat před podvybitím. Normálně bych ho nechal připojený k baterce během ježdění. Jakmile kterýkoli z článku klesne k 3,5V (popravdě si nejsem jistý na kolik je tam přesně nastavená hranice, dá se změnit) tak to začne hlasitě pípat. To je signál k ukončení jízdy.