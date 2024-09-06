# <p style = "text-align:">Záródolgozat</p>
<br><br><br><br><br><br><br><br>
## <p style = "text-align: right"> Rebman Fanni Viktória </p>
<br><br><br><br><br><br><br>
### <p style = "text-align: center ">Budapest</p>  


#### <p style = "text-align: center">2020</p>

<br><br><br><br><br><br><br><br>
<br><br><br><br><br><br><br><br>

---
## <p style=" text-align: center "> Budapesti Komplex Szakképzési Centrum <br> Weiss Manfréd Szakgimnáziuma, <br>Szakközépiskolája és Kollégiuma 
<br><br><br><br><br><br><br>
### <p style="text-align: center"> Thesis Quest</p> 
<br><br><br><br><br><br><br>
#### <p> Témavezető:<span style ="margin-left: 80%"> Készítette: <span></p> 

<p> Englert Ervin<span style ="margin-left: 73%">Rebman Fanni Viktória <br>
<span style="margin-left: 73%">Szoftverfejlesztő OKJ –<span>  
esti tagozat  <span></p> 
<br><br><br><br><br><br><br><br><br>

### <p style = "text-align: center ">Budapest</p>  
#### <p style = "text-align: center">2020</p>
---

## <p style = "text-align: center ">Tartalomjegyzék</p>

1. [Bevezetés](#bevezetés)
   - 1.1. [Köszönetnyilvánítás](#köszönetnyilvánítás)
   - 1.2. [Témaválasztás](#témaválasztás)
   - 1.3. [Témaválasztás indoklása](#témaválasztás-indoklása)
2. [Felhasználói dokumentáció](#felhasználói-dokumentáció)
   - 2.1. [Rendszerkövetelmények](#rendszerkövetelmények)
   - 2.2. [A program elindítása](#a-program-elindítása)
     - 2.2.1. [Program indítása exe fájlal](#program-indítása-exe-fájlal)
     - 2.2.2. [Program indítása fejlesztőkörnyezetből](#program-indítása-fejlesztőkörnyezetből)
   - 2.3. [Főmenü](#főmenü)
     - 2.3.1. [Start gomb](#start-gomb)
     - 2.3.2. [High Scores gomb](#high-scores-gomb)
     - 2.3.3. [Exit gomb](#exit-gomb)
   - 2.4. [A játék](#a-játék)
     - 2.4.1. [Játéktér](#játéktér)
     - 2.4.2. [Szövegdoboz](#szövegdoboz)
     - 2.4.3. [Irányítás](#irányítás)
     - 2.4.4. [Küldetések és Nem Játszható Karakterek](#küldetések-és-nem-játszható-karakterek)
     - 2.4.5. [Vége képernyő](#vége-képernyő)
   - 2.5. [Dicsőségtábla](#dicsőségtábla)
3. [Fejlesztői dokumentáció](#fejlesztői-dokumentáció)
   - 3.1. [Fejlesztői környezet](#fejlesztői-környezet)
   - 3.2. [Fájlok, osztályok, főprogramok, alprogramok, változók](#fájlok-osztályok-főprogramok-alprogramok-változók)
     - 3.2.1. [run.py](#runpy)
     - 3.2.2. [main_menu.py](#main_menupy)
     - 3.2.3. [name.py](#namepy)
     - 3.2.4. [game.py](#gamepy)
     - 3.2.5. [player_class.py](#player_classpy)
     - 3.2.6. [npc1.py, npc2.py, npc3.py, npc4.py, npc5.py](#npc1py-npc2py-npc3py-npc4py-npc5py)
     - 3.2.7. [hitbox.py](#hitboxpy)
     - 3.2.8. [gg.py](#ggpy)
     - 3.2.9. [high_score.py](#high_scorepy)
   - 3.3. [Fontosabb kódrészletek](#fontosabb-kódrészletek)
     - 3.3.1. [Gombok](#gombok)
     - 3.3.2. [Felhasználónév input](#felhasználónév-input)
     - 3.3.3. [Karakter mozgása, animációja](#karakter-mozgása-animációja)
     - 3.3.4. [Küldetések és NJK-k](#küldetések-és-njk-k)
     - 3.3.5. [Dicsőséglista](#dicsőséglista)
   - 3.4. [Grafikus elemek és képek](#grafikus-elemek-és-képek)
     - 3.4.1. [Főmenü háttérkép](#főmenü-háttérkép)
     - 3.4.2. [Játéktér kialakítása](#játéktér-kialakítása)
     - 3.4.3. [Szövegdoboz](#szövegdoboz)
     - 3.4.4. [Játékos karakter](#játékos-karakter)
     - 3.4.5. [Nem Játékos Karakterek](#nem-játékos-karakterek)
   - 3.5. [Betűtípusok](#betűtípusok)
     - 3.5.1. [Menüben felhasznált betűtípus](#menüben-felhasznált-betűtípus)
     - 3.5.2. [Játékban felhasznált betűtípus](#játékban-felhasznált-betűtípus)
   - 3.9. [Tesztdokumentáció](#tesztdokumentáció)
4. [Fejlesztési lehetőségek](#fejlesztési-lehetőségek)
5. [Irodalomjegyzék](#irodalomjegyzék)

---

## <p style ="text-align: center">Bevezetés</p>

### 1.1. Köszönetnyilvánítás

Szeretném megköszönni Englert Ervin tanár úrnak, hogy segített a program elkészítésében. Az ő segítsége nélkül nem jöhetett volna létre a játék. Továbbá szeretném megköszönni Kiss Viktornak, aki szintén végig támogatott az egész OKJ képzés alatt.

### 1.2. Témaválasztás

A záródolgozatom témája egy pixelgrafikus kalandjáték, amelyben a játékos küldetésekkel nyerheti meg a játékot. A történet szerint a karakter elveszítette a záródolgozatát, amelynek lapjai küldetések során szerezhetők vissza.

### 1.3. Témaválasztás indoklása

A pixelgrafikus játékok különleges helyet foglalnak el a szívemben, gyerekkorom miatt. Szeretnék később is pixelgrafikus játékokat fejleszteni, és ezzel a projekttel szeretném ezt az irányt megalapozni.

---

## 2. Felhasználói dokumentáció

<br>

### 2.1. Rendszerkövetelmények

Minimális rendszerkövetelmény:
-** CPU:** Intel Core i3
- **RAM:** 4 GB
- **HDD:** 1 GB
- **VGA:** 64 MB integrált
- **Operációs rendszer:** Windows 7

Optimális rendszerkövetelmény:
- **CPU:** Intel Core i5
- **RAM:** 8 GB
- **HDD:** 2 GB
- **VGA:** 4 GB integrált
- **Operációs rendszer:** Windows 10

### 2.2. A program elindítása

A programot a  [https://drive.google.com/open?id=1jqPG-
KUnkxn8r1OZCprWFC0x90430u5W](https://drive.google.com/open?id=1jqPG-KUnkxn8r1OZCprWFC0x90430u5W). linkre kattintva érheti el. Amennyiben a programot 
exe fájllal szeretné elindítani, akkor a ThesisQuest_exe.zip fájlt töltse le, csomagolja ki, 
ellenkező esetben a ThesisQuest.zip fájlal járjon el hasonló módon.

#### 2.2.1. Program indítása exe fájlal

 program elindításához a ThesisQuest nevű mappában található run.exe fájlra az egér bal 
gombjával duplán kattintson.

#### 2.2.2. Program indítása fejlesztőkörnyezetből

A programot egy python fejlesztőkörnyezetben is futtathatja. Ez a Linux, továbbá az IOS 
operációs rendszerrel rendelkezők számára is lehetővé teszi a program futtatását. 
Amennyiben fejlesztőkörnyezet által szeretné futtatni a programot, a Thonny 
fejlesztőkörnyezet ajánlott a játék futtatására. A Thonny-t letöltheti a https://thonny.org/ 
weboldalról, majd az oldalon található telepítési útmutatókkal, telepítheti a szoftvert. Ezek 

<center>

 ![cmd]([cmd.png](https://raw.githubusercontent.com/lacko186/Markdown_/main/markdown/cmd.PNG)) 

</center>

</center>
<center>
*Windows10 operáációs rendszer esetében a Pygame installálása*
 </center>

A telepítést követően, ha a Thonny-t megnyitja, majd abból megnyitja a ThesisQuest mappa 
run.py fájlját, majd az F5 billentyűt lenyomja, a program elindul. 

### 2.3. Főmenü

A program indításakor megnyílik egy ablak, amelyben rögtön a játék főmenüjét láthatjuk. 
Felül látható a játék ikonja, valamit mellette a címsorban a program neve. Alul a főmenüben 
található ismét a játék címe, valamint három gomb, melyekre az egérrel kattintva lesznek 
elérhetők az adott funkciók, illetve menüpontok:  
- Start
- High Scores
- Exit

<center>

![1]([cmd.png](https://raw.githubusercontent.com/lacko186/Markdown_/main/markdown/cmd.PNG)

</center>

</center>

#### 2.3.1. Start gomb

A start gombra való kattintással a program a játék indítását fogja végrehajtani, de ezt 
megelőzően először a felhasználónak egy maximum 8 karakter hosszúságú nevet kell 
megadnia, mellyel felkerülhet a dicsőséglistára, a megoldott küldetéseinek számával együtt. 

<center>

![2]([2.png](https://raw.githubusercontent.com/lacko186/Markdown_/main/markdown/2.PNG)

</center>
A játékosnév megadásához először bele kell kattintani a név megadására szolgáló négyzetbe 
az egérrel. Akkor tud bele írni, ha a négyzet kerete világosról sötét színűre változik 

<center>

![3]([3.png](https://raw.githubusercontent.com/lacko186/Markdown_/main/markdown/3.PNG)

</center>

A felhasználónév megadása után ismét egy START nevezetű gombra kattintva, a játék 
immár ténylegesen elindul. 
#### 2.3.2. High Scores gomb

A HIGH SCORE gombra kattintva megtekintheti a játékkal játszottak dicsőséglistáját. A 
lista tartalmazza a játék kezdete előtt megadott felhasználóneveket, illetve a játék során 
elvégzett küldetések számát. 

<center>

![4]([4.png](https://raw.githubusercontent.com/lacko186/Markdown_/main/markdown/4.PNG)

</center>

#### 2.3.3. Exit gomb

Az EXIT gombra kattintva kiléphet a programból. 
---

### 2.4. A játék

A játék elindulásakor az ablak felső részén kap helyet maga a játéktér, alul pedig egy általam 
„szövegdoboz” néven futó rész, mely a játék során kiírja a játékban helyet kapó 
párbeszédeket és egyéb szövegeket

<center>

![5]([5.png](https://raw.githubusercontent.com/lacko186/Markdown_/main/markdown/5.PNG)

</center>

#### 2.4.1. Játéktér

A játéktér egy iskolának ad otthont, melyben különböző helyiségek vannak, mindegyikhez 
egy - egy NJK (nem játszható karakter). Mindegyik NJK a maga helyiségénél áll, ezzel 
reprezentálva azt is, hogy hol kell megcsinálni az adott küldetéseket. 
<center>

![6]([6.png](https://raw.githubusercontent.com/lacko186/Markdown_/main/markdown/6.PNG)

</center>

#### 2.4.2. Szövegdoboz

A szövegdobozban jelenik meg minden, amit az NJK-ek mondanak, illetve a küldetésekhez
tartozó tárgyak szövegei, ha a játékos elég közel van az NJK-hoz, illetve a tárgyhoz 

<center>

![7]([7.png](https://github.com/lacko186/Markdown_/blob/main/markdown/7.PNG)

</center>

#### 2.4.3. Irányítás

A játékost a billentyűzeten található nyíl gombokkal lehet irányítani. A karakter az adott 
billentyű lenyomásával, az ahhoz megfelelő irányba fog elmozdulni. A játék menete alatt 
más gombok használatára vagy az egérre nincs szükség. A karakter csak egyetlen egy 
tempóban tud haladni. 

<center>

![8]([8.png](https://github.com/lacko186/Markdown_/blob/main/markdown/8.PNG)

</center>

#### 2.4.4. Küldetések és Nem Játszható Karakterek

A játékban öt küldetés van, ezeket csak egy adott sorrendben lehet elvégezni, ezáltal csak 
akkor válik elérhetővé a következő küldetés, ha az előzőt már teljesítette a játékos. A 
küldetések alatt az NJK-k elmondják a feladatot, melyet a karakternek teljesítenie kell, hogy 
leadhatja a záródolgozatát. A játék során négy normális küldetés van, az ötödik, egyben 
utolsó küldetés akkor válik aktívvá, ha a játékosnak sikerül az összes küldetést megcsinálnia. 
Itt a záródolgozatot kell leadni.  
A küldetések elvégzéséhez a karakternek megfelelő távolságra kell lennie az NJK-tól, 
valamint a tárgyaktól, hogy haladjon a küldetésekkel, és megjelenítse a hozzájuk tartozó 
szöveget. Azok az NJK-k, akiknek a küldetése nem aktív, vagy már elkészült, jelezni fogják, 
hogy a jelenleg aktív küldetést csinálja.  
A küldetések működése rendkívül egyszerű. A karakter a soron következő NJK-val kell 
beszélnie, aktiválj a küldetést, majd, ha megfelelő tárgy is megjeleníti a szövegét, akkor már 
csak vissza kell menni az adott NJK-hoz, hogy befejezze a küldetést. 

<center>

![9]([9.png](https://github.com/lacko186/Markdown_/blob/main/markdown/9.PNG)

</center>

#### 2.4.5. Vége képernyő

Ha sikerül az összes küldetés, akkor a játéknak vége, a felhasználó nyert, majd megjelenik a 
vége képernyő. Itt található egy felirat, mely szerint a játékos nyert, valamit egy EXIT 
feliratú gomb, ami a főmenüben lévőhöz hasonlóan működik, tehát ha az egérrel rákattint a 
felhasználó, akkor kilép a programból. 



<center>

![10]([10.png)](https://github.com/lacko186/Markdown_/blob/main/markdown/10.PNG)

</center>

### 2.5. Dicsőségtábla

A dicsőságtáblát a főmenüben a HIGH SCORES gombra kattintva válik elérhetővé. Az ablak 
tetején helyezkedik el a cím szöveg, alatt pedig maga a dicsőségtábla, amely tartalmazza 
azoknak a felhasználóknak a nevét, valamint teljesített küldetéseinek számát rangsorolva. A 
dicsőségtábla a három legjobb játékos adatait tartalmazza, amennyiben ennél kevesebb játkos 
játszott, a legjobb kettő, egy játékos eredményeit mutatja, vagy egyet se, ha még egy játékos 
se ért el eredményt.

<center>

![11]([11.png](https://github.com/lacko186/Markdown_/blob/main/markdown/11.PNG)

</center>

---

## 3. Fejlesztői dokumentáció

### 3.1. Fejlesztői környezet

A következő szoftvereket és fejlesztői eszközöket használtam a játék fejlesztése során:

  <span style="margin-left: 10%" >Python 3.8.0: </span>
  <span style="margin-left: 40%" >A programomat Python nyelven írtam</span>
  
  <span style="margin-left: 10%" >Pygame: </span>
  <span style="margin-left: 60%" >Egy multimédiás könyvtár</span> 
  <span style="margin-left: 60%" > amely lehetővé teszi a grafikus elemek kezelését.</span>
  
        
  <span style="margin-left: 10%" >IDLE: </span>
  <span style="margin-left: 45%" >A Python hivatalos fejlesztői környezete.</span>
  
   <span style="margin-left: 10%" > Paint és Adobe Photoshop 2020:</span>
  <span style="margin-left: 30%" > A grafikus elemek </span> <span style="margin-left: 60%" >létrehozására és szerkesztésére.</span>
</span>

  <br>

### 3.2. Fájlok, osztályok, főprogramok, alprogramok, változók

AA játék több fájl által működik. A fájlokban lévő osztályok, fő- és alprogramok egymásba 
importálása lehetővé teszi a játék zavartalan működését, miközben elszeparálódnak az 
egyes részek. 

<center>

![12]([12.png)](https://github.com/lacko186/Markdown_/blob/main/markdown/12.PNG)
</center>

#### 3.2.1. run.py

A run fájl használatát és annak ötletét egy internetes tutorialvideo-ból vettem, és a játék 
GitHubra felöltött változatát használtam fel, és azt alakítottam kicsit. 
https://github.com/techwithtim/Tower-Defense-Game/blob/master/run.py 
A run.py a játék alapköve, amelyben inicializálódik a screen nevű változó, azaz az ablak, 
amelyet az összes többi osztályba fel lesz használva, továbbá itt állítódik be a program 
ikonképe, és az ablakban megjelenő cím, így a továbbiakban ezeket sem kell beállítani. 
Az alapvető inicializálások után a menu almappából a main_menu.py fájlból beimportálja 
a *MainMenu* osztályt, azt *main_menu* néven inicializálja, oda adja neki a screen változót, 
végül futtatja az osztály *run* nevű programját.

<center>

![13]([13.png](https://github.com/lacko186/Markdown_/blob/main/markdown/13.PNG))

</center>

#### 3.2.2. main_menu.py
A *run.py* futtatása meghívja a *main_menu.py* fájlt, amelyben a játék főmenüjének részei 
találhatóak: egy *MainMenu* nevű osztály, amiben inicializálódnak a *MainMenuben* használt 
változók. Ezek a változók az ablak szélessége *(self.width)*, magassága *(self.height)*, a 
képernyőn megjelenő háttérkép *(self.bg)*, valamint cím *(self.title)*, a gombokhoz tartozó 
képek*(self.start, button, self.hs_button, exit_button)*, négyzetek *(self.button_s, self.button_hs, self.button_e)*, végül maga a képernyő (screen), amely a run.py fájlban lett 
korábban inicializálva, de a MainMenu meghívásakor ezt tovább adta. 

<center>

![14]([14.png](https://github.com/lacko186/Markdown_/blob/main/markdown/14.PNG)

</center>

A *run* a főmenühöz tartozó főprogram, amelyben egy végtelen ciklus van, amely addig 
megy, amíg a felhasználó ki nem lép a programból, akkor a *while run*, run nevű logikai 
változója HAMIS értéket vesz fel, így nem fut tovább a ciklus. 

<center>

![15](https://github.com/lacko186/Markdown_/blob/main/markdown/16.PNG))

</center>

A *Draw* egy olyan alprogram, amelyben felsorolódnak a képernyőre kirajzolandó képek, 
szövegek, egyéb síkidomok, mint például a gombokhoz használatos négyzetek. Ennek végén 
található a *pygame.display.update* nevű parancs, mely frissíti a képernyőt, ezzel megjelenítve a 
képeket. Ezeket a run programban meghívva lehet látni. 

<center>

![17](https://github.com/lacko186/Markdown_/blob/main/markdown/17.PNG)

</center>
## 3.2.3.  name.py 
A *MainMenu* osztály *run* programjában van egy eventhez kötött egérlenyomás, mely 
meghívja a game almappa name.py fájl Main nevű osztályát és annak összes eljárását. 
A Main osztályban inicializálódik a képernyő *(screen)*, annak szélessége *(width)*, 
magassága *(height)*, az inputboxhoz tartozó színek, egy, amikor aktív az 
inputbox *(color_active)* és egy, amikor inaktív *(color_inactive)*. A képernyő háttere *(bg)*, a 
cím *(title)*, egy START gomb képe *(start_button)*, és a hozzá tartozó négyzet *(button_s)*, és 
végül egy betűtípus *(font)*. 
<center>

![18]([18.png)](https://github.com/lacko186/Markdown_/blob/main/markdown/18.PNG)

</center>
A *Main* osztály mellett helyet kapott még egy osztály, aminek a neve
*InputBox* , ebben 
inicializálódik, és határozódik meg az az inputbox, amibe a felhasználó megadj a nevét. Itt 
meg lett határozva egy négyzet *(textbox)*, a képernyő *(screen)*, az aktív- és inaktív színek, a 
betűtípus, egy *text* nevű üres string, és egy txt_surface, amely egy lerenderelt szöveg az 
adott betűtípussal, és egy *active* logikai változó, ami meghatározza, hogy az inputbox akív 
e, tehát a felhasználó tud bele írni, vagy sem. 
<center>

![19]([19.png)](https://github.com/lacko186/Markdown_/blob/main/markdown/19.PNG)

</center>

A *Handle_event* alprogram kezeli az inputboxba a szövegbevitelt. A *Draw* alprogram 
rajzolj a ki az inputboxot és a rerenderelt szöveget. 
A Main run programjában van egy végtelen ciklus, ahol a főmenühöz hasonlóan kezeli a 
gomb működését, de csak akkor nyomhat rá a felhasználó, ha a felhasználónevet tartalmazó 
text változó nem üres. Ekkor a *game.py* fájl *Game* nevű osztályát inicializálja, és megadja 
neki a *screen*, és az *InputBox text* változóját, azaz a játékos nevét. Továbbá itt hivódik meg 
a Main Draw programja, és az InputBox alprogramjai. 

 

## 3.2.4. game.py 
A *game.py* fájlban van a *Game* osztály, ahol inicializálódik a játékhoz szükséges változók 
és a többi osztály, amelyek szükségesek a játék működéséhez. A képernyő(*screen*), annak 




 

szélessége(*width*), magassága(*height*), a játékon belül használt betűtípus(*font*), az 
óra(*clock*), egy logikai változó, mely a karakter mozgásával és fizikájában kap 
szerepet(*collide*), egy int változó, ami a teljesített küldetéseket számolja(*score*), és egy 
olyan logikai változó, ami azt vizsgálja, hogy a játékos megnyerte e a játékot vagy 
sem(*win*). Ezek alatt jönnek a beimportált osztályok inicializálása, hogy fel lehessen őket 
használni, a Player(*player*), a HitBox(*hitbox*), a Textbox(*textbox*), NPC1(*npc1*), 
NPC2(*npc2*), NPC3(*npc3*), NPC4(*npc4*), NPC5(*npc5*). 

<center>

![20]([20.png)](https://github.com/lacko186/Markdown_/blob/main/markdown/20.PNG)

</center>

A *run* program meghívja az összes olyan programot, amit felhasznál a játék, a képernyőre 
rajzolás, a küldetések, a teljesített küldetésének számának számolása, a karakter mozgása 
és fizikai hatása a környezetére, valamint annak eldöntése, hogy a játékos megnyerte e a 
játékot, vagy sem. 
A *Draw*-ban van felsorolva minden, amit ki kell rajzolni a képernyőre, a háttérkép, a 
karakter, a textbox a képernyő aljára, az NJK-khoz tartozó kiírandó szövegek, végül frissíti 
a képernyőt, hogy ezeket látni lehessen a program futtatásakor. 

<center>

![21]([21.png)](https://github.com/lacko186/Markdown_/blob/main/markdown/21.PNG)

</center>

A *Score* alprogram számolj a teljesített küldetések számát. Ha egy küldetés elkészül, akkor 
a *score* értéke változik, vagyis eggyel növekszik. Ha az utolsó küldetést is teljesítette a 
játékos, akkor a win változó IGAZ értéket vesz fel. 

<center>

![22](https://github.com/lacko186/Markdown_/blob/main/markdown/22.PNG)

</center>

A *Win* alprogram hívja meg a játék vége képernyőjét. Ha a *win* IGAZ, akkor a *game* almappából a *gg.py* nevű fájl *GG* osztályát beimportálja, iniciálja azt gg néven, majd annak 
főprogramját, a *run-t*, futtatja, végül frissíti a képernyőt. 

<center>

![23](https://github.com/lacko186/Markdown_/blob/main/markdown/23.PNG)

</center>

A *Write*-ban fájlkezelés történik. A *game* almappába, ha nem létezik kreál, ha létezik 
hozzáfűz a *scoreboard.txt* nevű fájlhoz, melyet f néven használ a program a későbbiekben. 
A játékosnevet, valamint a teljesített küldetések számát írja bele a fájlba. A fájlba írás csak 
a program bezárásakor, pontosabban közvetlenül azelőtt történik, különben, ha a többi 
alprogrammal együtt lenne meghívva, akkor minden egyes lefutáskor/frissítéskor 
belekerülne a játékos neve. 

<center>

![24](https://github.com/lacko186/Markdown_/blob/main/markdown/24.PNG)

</center>

#### 3.2.5. player_class.py

A *Player* osztályban vannak a karakterhez tartozó változók, az x, y, szélesség(width), 
magasság(*height*), a játékos mozgási sebessége(*vel*), irányokat jelölő logikai változók (*left,*


 

*right, up, down)*, egy int típusú változó, ami az animációkat számolja (*walking*), egy olyan 
logikai változó, ami azt nézni, hogy a karakter egyhelyben áll e, vagy mozog(standing), a 
karakterhez tartozó hitbox, ami egy négyzet, és végül négy lista, amelyek a négy irány 
szerint különíti el a karakter animációihoz tartozó képeket. 
A *Draw* alprogram kezeli a játékos animációját, amely a játékon belül megjelenik. 

<center>

![25](https://github.com/lacko186/Markdown_/blob/main/markdown/25.PNG)

</center>

#### 3.2.6. npc1.py, npc2.py, npc3.py, npc4.py, npc5.py

Az összes NJK-nek külön fájlban van személyre szabottan osztály, NPC plusz a hozzájuk 
rendelt sorszám néven *(NPC1, NPC2, NPC3, NPC4, NPC5)*. Az első négynél azonosak a 
változók is, csak értékekben térhetnek el, az ötödik picit eltérő, hiszen az akkor lesz aktív, 
ha az összes korábbi küldetés kész van, így vele elég egyszer beszélni, nem kell az 
előzőkhez hasonlóan egy tárgyat megkeresni, csupán leadni az elvégzett küldetést. 

 

Mindegyikben van egy *x, y*, egy screen, egy x és y pont a textboxban*(tb_x, tb_y)*, egy 
szélesség(*width*), egy magasság(*height*), a betűtípus(*font*), egy activeline nevű üres string 
változó, egy npc_count nevű integer, a karakter hitboxa(*hitbox*), egy lines nevű listában az 
adott karakter szövegei, a küldetésekhez tartozó tárgy hitboxa(*item*), a tárgy 
szövege(itemline), a küldetés aktívságát jelző logikai változó(*active*), az tárgy aktívságát -
(*itemactive*), a küldetés elkészültségét(*done*) jelző logikai változók, valamint egy, ami azt 
jelzi, hogy a tárgy meg van e(*itemfound*). Az NPC1 osztályt kivéve, van még egy változó a 
többi osztályban. Az előtte levő  NJK osztályát beimportálja, a done változó miatt.   

<center>

![26](https://github.com/lacko186/Markdown_/blob/main/markdown/26.PNG)

</center>


Az ötödik NJK kicsit másképp működik, mint a többi. Itt nincs szükség küldetés béli 
tárgyhoz, se ahhoz tartozó egyéb változókra, a szövege is kevesebb.

<center>

![27](27.png)

</center>

#### 3.2.7. hitbox.py

A hitbox.py fájlban van a HitBox osztály. A hitboxok a játékban fontos helyet foglalnak el, 
mivel ezek által lesz fizika a játékban. Az osztály használj a Player osztályt(*player*), a 
*collide* változót a *Game* osztályból, valamint a screent. Van egy *hitboxes* nevű lista, ami 
tartalmazza a játéktérben található összes hitboxot. 
A *Collide* program a karakter hitboxa és a hitboxes lista elemeit felhasználva eldönti, hogy 
a collide mikor IGAZ, és ezt az IGAZ, vagy éppen HAMIS értéket felhasználva történik 
meg a játékos mozgása a *Moving* programban. 

<center>

![28](https://github.com/lacko186/Markdown_/blob/main/markdown/28.PNG)

</center>

#### 3.2.8. gg.py

A *GG* osztályban az alapvető adatok, hasonlóan a korábbiakhoz lesznek megadva, 
képernyő(*screen*), magasság(*height*), szélesség(*width*), egy exit gomb képe(*button*) és a 
hozzá tartozó négyzet(*b_hitbox*), egy háttérkép(*bg*), és végül egy cím képe (*title*) 
A *Draw* alprogram kirajzoltatja a háttérképet, a címet, a gomb képét és négyzetét, amit a 
run meghív, és a gombot használhatóvá teszi. 

<center>

![29](https://github.com/lacko186/Markdown_/blob/main/markdown/29.PNG)

</center>


#### 3.2.9. high_score.py

A high_score.py fájlban van a *HighScore* osztály, amely tartalmazza a screen változót, a 
képernyő magasságát(*height*), szélességét(*width*), a betűtípust(*font*), a háttérképet(*bg*), egy 
top nevű üres listát. Továbbá hat darab üres string változó, a top három játékos nevének és 
pontszámának, továbbá mindegyiknek egy képernyőre kiíratható változataik. 
A *run* alprogram meghívja a *Draw* és a Read alprogramokat. A Draw alprogram kirajzoltat 
minden a képernyőre, A Read alprogramban történik a fájlból olvasás, és a dicsőséglista 
működése. 

<center>

![30](https://github.com/lacko186/Markdown_/blob/main/markdown/30.PNG)

</center>

### 3.3. Fontosabb kódrészletek

#### 3.3.1. Gombok

A gombok működést a következő linken található oldalról vettem, és felhasználtam. 
https://stackoverflow.com/questions/46390231/how-to-create-a-text-input-box-with-
pygame 

 

A programon belül több gomb is helyet kapott, melyekre az egérrel kattintva elérhetőek 
lesznek az adott funkciók. Ezek működése megegyezik. Az egér bal gombjának 
lenyomásakor a kurzor x és y koordinátája az adott gomb x, y koordinátájára, ugyanakkora 
szélességűre és magasságúra rajzolt négyzeten belül van, akkor a megadott esemény 
történik: példádul kilép a program, láthatjuk a dicsőséglistát, vagy elindíthatjuk a játékot.

<center>

![31](https://github.com/lacko186/Markdown_/blob/main/markdown/31.PNG)

</center>

#### 3.3.2. Felhasználónév input

A felhasználónév inputboxának működését a következő linken találtam, és azt alkalmaztam. 
https://stackoverflow.com/questions/46390231/how-to-create-a-text-input-box-with-
pygame 

 

A főmenüben a START gombra kattintás meghívja a *name.py* fájl főprogramját. A 
felhasználónév megadásához egy külön osztályt használtam, azon belül is kettő eljárást. Az 
elsőben, ha az egérrel az előre megrajzolt inputboxba kattintunk, akkor az aktív állapotba 
kerül, ezt a szegély színének megváltozása jelzi a felhasználónak. Alaphelyzetben az 
inputbox nem aktív ezért, ha belekattintunk aktív lesz, viszont következő kattintásra ismét 
inaktív lesz. Amennyiben az inputbox aktív állapotban van, akkor a felhasználó 
alfanumerikus, valamint numerikus karaktereket vihet be, a megfelelő billentyű 
lenyomásával. A *text* nevű változó kezdetben üres string típusú változó, amelyhez a 
lenyomott billentyű karaktere hozzáadódik. A BACKSPACE/ TÖRLÉS billentyűvel a text 




változóban lévő karakterek törlődnek a végéről kezdődően. Amennyiben a szöveg hosszabb 
8 karakternél, a legutolsó karakter törlődik. A *txt_surface* újrarendereli a textet, amit a 
második eljárásban kiíródik grafikusan a képernyőre, hogy a felhasználó láthassa a begépelt 
felhasználónevet és annak jelenlegi állapotát, és az inputboxot is megrajzolja. 

<center>

![32](https://github.com/lacko186/Markdown_/blob/main/markdown/32.PNG)

</center>

#### 3.3.3. Karakter mozgása, animációja

A karakter mozgásának animációja a *Player* osztályhoz tartozó *Draw* alprogramban megy 
végre. Az osztály inicalizálásakor a *WalkLeft, WalkRight, WalkUp, WalkDown* listákban 
betöltődnek az adott irányhoz tartozó képek az álló, egyik láb, másik láb sorrendben.  
Ha a *walking* + 1 nagyobb egyenlő kilencnél, akkor a *walking* nullára állítódik, ezzel 
egyfajta felső határértéket szabva. a kilences számot elosztva az egyirányban felhasználható 
képek számával, ami három, hármat kapunk, ennyivel kell majd elosztani a walkingot, így 
ennyiszer fog mutatni képet 1 animáció alatt, lényegében ez a változó számolja az 
animációk számát. 
Ezalatt következik a karakter igazi „animálása”. Ha a karakter nem áll, azaz mozgásban 
van, és az adott irányhoz tartozó logikai változó értéke IGAZ, akkor az azonos irányhoz 
tartozó lista elemit rajzolja ki, a fentebb említett módszerrel, vagyis a *walking* hárommal 
való osztásával biztosítva lesz, hogy egy kép háromszor látható minden animációkor. 



 

Ha a karakter nem mozog, vagyis áll, hogy abba az irányba álljon arccal előre, ahogy 
megállt, ismét az irányokat megadó logikai változók határozzák meg a lehetőségeket, és 
minden irány animációjának legelső képét mutatják, mivel az az álló kép. 
Ezek mellett szükséges volt egy ötödik állóképre, mivel enélkül a játék indításakor a 
karakter nem látszódna a legelső mozgásig, mivel csak akkor mutatna képet, ha bármelyik 
irány IGAZ. A játék indításakor a karakter nem mozog, így az álló képek között kell lennie, 
ha semelyik irányba se állt meg, mivel nem is ment azelőtt sehova. Ilyenkor a karakter lefele 
néző, álló képe jelenik meg. 
Mivel a karakterrel együtt mozog a hitboxa, ezért minden egyes elmozduláskor újra rajzolja 
a *hitboxot*.

<center>

![33](https://github.com/lacko186/Markdown_/blob/main/markdown/33.PNG)

</center>

A karakter valódi mozgása a *HitBox* osztály *Moving* alprogramjában történik. Mivel a 
pályatér tele van „bútorokkal” és „falakkal”, ezért nem lenne jó, ha a karakter ezeken a 
fizika törvényeit meghazudtolva, átsétálna. Az osztály változóinak inicalizálásakor 
meghatározott hitboxes nevű listában lett felsorolva a pályán található összes elem hitboxa, 
amelyeken nem kéne átsétálnia a karakternek. A *Collide* alprogramban lefut egy ciklus, ami 
a *hitboxes* lista elemein megy végig. A *hitbox* alapvetően egy négyzet, amelyet az adott 
entitás köré rajzolnak. A *colliderect* parancs két négyzet átlapolását vizsgálja, jelen esetben, 
ha a karakter hitboxa beleütközik a játéktéren elhelyezett bármelyik másik hitboxba, akkor 
a *collide* változó IGAZ értéket vesz fel. 

<center>

![34](https://github.com/lacko186/Markdown_/blob/main/markdown/34.PNG)

 </center>

A *Moving* alprogramban a *keys* lesz a lenyomott gomb. Ha a *collide* HAMIS értékű, akkor 
az adott irányt jelző gomb (bal, jobb, föl, le) van lenyomva, és az x és y tengely helyzetében 
a maximum távolság nagyobb, mint a játékos helyzete(*x, y*), plusz a sebessége (*vel*), akkor 
ha balra akar menni, a játékos x értéke egyenlő lesz az x érték mínusz sebességgel. A 




 

jobboldal esetében ez plusz lesz, mivel pythonban az x és y tengely nullás értéke a képernyő 
bal felső sarka, így balra és felfele csökken, lefele és jobbra nő az érték. Ennek tudatában a 
föl és le irányok ugyanígy működnek, csak az y tengelyen. A karakter animációja az ahhoz 
tartozó irányokról elnevezett logikai változók állapotától függően mennek végbe, ilyenkor 
az adott irányba IGAZ értéket vesznek fel, a többi HAMIS, valamint az egyhelyben állás 
(*standing*). Ha áll a karakter, akkor ennek fordítottja történik, valamint a *walking* érétke 0 
lesz újra, hogy megfelelően mutassa az animációkat, ha újra elindul a karakter. 

<center>

![35](https://github.com/lacko186/Markdown_/blob/main/markdown/35.PNG)

</center>

*(A kódrészletet két képrészletben tudtam itt megjeleníteni, ezért az elágazásokban csúszások 
lehetnek, egyes részletek akár kétszer is szerepelhetnek)*

 

Ha a *collide* IGAZ, vagyis a játékos belemegy valamibe, akkor az adott irányhoz képest 
ellentétes irányba fog elmozdulni, így a karakter nem tud belesétálni a másik hitboxba, 
hanem mindig visszamegy oda, ahol összeért a másik hitboxal. 

<center>

![36](https://github.com/lacko186/Markdown_/blob/main/markdown/36.PNG)

</center>

*(A kódrészletet két képrészletben tudtam itt megjeleníteni, ezért az elágazásokban csúszások 
lehetnek, egyes részletek akár kétszer is szerepelhetnek)*
#### 3.3.4. Küldetések és NJK-k

Minden Nem Játszható Karakternek külön osztály és küldetés lett meghatározva, 
lényegében hasonló, mégis egy kicsit eltérő módon. A legelső és a legutolsó küldetés lett a 
leginkább eltérő tartalmilag. 
Alapvetően az egyes küldetés aktív, így amikor a karakter odamegy hozzá, és a hitboxaik 
összeérnek, akkor az *activeline* alapból a nullás indexű szöveg, ami a küldetést mondja el. 
Ha a karakter hitboxa összeér az NJK hitboxával, akkor kiírja az activeline-t, és az 
npc_count értéke nő eggyel. Ha már egynél többször beszélt vele a karakter, akkor az 
itemactive IGAZ értékre változik, tehát a küldetés tárgy elérhetővé válik a karakter számára. 
Ha ez megtörténik, akkor, ha a játékos hitboxa összeér a tárgyéval, akkor az itemline 
kiíródik a képernyőre, és az *itemfound* IGAZ értéket vesz fel, tehát a karakter megtalálta a 
keresett tárgyat. Ha megtalálta, akkor az activeline vált az egyes indexű szövegre, ami a 
küldetés végét jelzi, az *npc_count* értéke ismét nulla lesz. Ha ezt követően beszél a játékos 
az NJK-val, akkor az *activeline* új szövegét írja ki, Ha beszélt vele, akkor a done változó 
IGAZ értéket vesz fel, tehát a küldetés kész van, az *npc_count* nő egyel, valamint az *active 
FALSE értéket vesz fel, hiszen már vége a küldetésnek. 
Ha a küldetés nem aktív, és a játékos mégis beszélne az NJK-val, akkor a *lines* lista második 
indexén lévő szöveg lesz az *activeline*, amiben arra kéri a játékost, hogy csináljon egy másik 
küldetést. 

<center>

![37](https://github.com/lacko186/Markdown_/blob/main/markdown/37.PNG)

</center>

A második, harmadik, negyedik küldetésnél annyi eltérés van, hogy csak akkor lesz aktív, 
ha az előző küldetés done változója IGAZ. 

<center>

![38](https://github.com/lacko186/Markdown_/blob/main/markdown/38.PNG)

</center>

Az ötödik küldetésnél egyszerűbb a helyzet. Ha kész a negyedik küldetés, akkor egyrészt 
az összes küldetés kész van, tehát az ő küldetése is kész van, ami az, hogy minden küldetést 
végezzen el. Ha aktív a küldetése, akkor a nullás indexű szöveg egyben a küldetés leadó 
szöveg. Amint a játékos karakter odamegy beszélni vele, az *activelinet* kiírja, a küldetés 
elkészül és többé nem akt*ív. Amíg nem lesz aktív az ő küldetése, addig az összes küldetés 
elvégzésére bíztatja a játékost. 

<center>

![39](https://github.com/lacko186/Markdown_/blob/main/markdown/39.PNG)

</center>


Minden NJK osztályához tartozik továbbá 
#### 3.3.5. Dicsőséglista
A dicsőséglista egy fájlban tárolódik el, amit a *Game* osztály *Write* alprogramja kezel. Ezt 
a *HighScore* osztály Read alprogramja olvassa. Egy *matrix* nevű kétdimenziós listába a fájl 
elemeit soronként beleírjuk. Így a *matrix* nevű listában lesznek listák, melyek egy 
karakternevet és egy pontszámot tartalmaznak. Ezeket a *strip*-el megszabadítja a sorvégi \ *n*-
től, és a sorok elemeit a pontosvessző karakter mentén választja szét, ezzel kétdimenziód 
listát, azaz mátrixot hozva létre. Ezek után a top nevű listában rendeződnek az adatok 
pontszám szerint, de mivel alapból növekvő sorrendbe rakná őket a *sorted*, ezért ezt meg 
kell fordítani, így lesznek a legmagasabb pontszámok a lista elején. Ebből adódóan, a top 3 
játékos kiíratásához az első három listán belüli lista adatira van csak szükség.  
A hibák elkerülése végett, ha nem volt még 3 név, akkor annyival kevesebb játékost fog 
megjeleníteni a dicsőségtábla, amennyiben még egyszer sem játszott a felhasználó a 
játékkal, akkor a dicsőségtábla üres.

<center>

![40](https://github.com/lacko186/Markdown_/blob/main/markdown/40.PNG)

</center>

*(A kódrészletet két képrészletben tudtam itt megjeleníteni, ezért az elágazásokban csúszások 
lehetnek, egyes részletek akár kétszer is szerepelhetnek)*

### 3.4. Grafikus elemek és képek
A programomban felhasznált képek egy része nem az én tulajdonomat képezik, én csupán 
kivágtam darabokat, majd képszerkesztésre alkalmas szoftverrel/szoftverekkel átszíneztem, 
esetleg kisebb átalakításokat vittem véghez. 

#### 3.4.1. Főmenü háttérkép

A főmenü háttérképéhez a játéktér falának színeit használtam fel, mivel a zöld kellemes és 
vidám szín, továbbá a karakter ruhája is hasonló árnyalatú. Miután elkészült, csináltam 
néhány tervet, hogy fog kinézni a menü véglegesen is. A színek a játéktér falán lévő két 
zöld árnyalatot használja. Az alapja egy egyszínű háttér, amire a másik színnel egy teli 
félkört helyeztem el. 

<center>

![41](https://github.com/lacko186/Markdown_/blob/main/markdown/41.PNG)

</center>

#### 3.4.2. Játéktér kialakítása

A játéktér kialakítása igényelte a rajzolt elemek közül a legtöbb időt. Minden faldarab, 
padlódarab, NJK, és berendezés egyesével lett lerakva, a játéktérre, mely sok átalakításon 
esett át. A helyiségek úgy lettek kialakítva, hogy mindegyikhez tartozzon egy NJK, és 
viszonylag könnyen tudjon mozogni a karakter. A játéktér alapjait a klasszikus Paintel 
csináltam, a színezéseket valamint a bútorokat Photoshoppal helyeztem el. 
<center>

![41](https://github.com/lacko186/Markdown_/blob/main/markdown/42.PNG)

</center>
#### 3.4.3. Szövegdoboz

A szövegdoboz ötlete régi pixelgrafikus játékok alapján jutott eszembe, ezért szerettem 
volna én is hasonló módszert alkalmazni.  

<center>

![42](https://github.com/lacko186/Markdown_/blob/main/markdown/42.PNG)

</center>

#### 3.4.4. Játékos karakter

A játékos karaktert egy több karaktert tartalmazó, internetről letöltött képből vágtam ki, 
színeztem ki, majd a mozgási állapotokat kivágtam. Photoshoppal eltávolítottam a kép 
hátterét, majd kisebb átdolgozásokat követően a színeket is megváltoztattam. Végül az 
animáció darabjait egyesével kivágtam 32x32 es méretre

<center>

![44](https://github.com/lacko186/Markdown_/blob/main/markdown/44.PNG)

</center>

#### 3.4.5. Nem Játékos Karakterek

A NJK-t a játékos karakterhez hasonlóan, a korábban már említett képről vágtam ki, 
változtattam a kinézetükön, és daraboltam szét, melyekből csak a jobbra vagy balra néző 
képeket használtam fel, az ötödik NJK estében szemből látható a karakter. Ezeket a 
játékoskarakteréhez hasonlóan szerkesztettem át. 

<center>

![45](https://github.com/lacko186/Markdown_/blob/main/markdown/45.PNG)

</center>


### 3.5. Betűtípusok
A játékban megjelenő szövegek betűtípusait a https://www.dafont.com/ linken elérhető 
weboldalról töltöttem le. Ezek a betűtípusok ingyenesen elérhetőek, valamint 
felhasználhatóak. 
 

#### 3.5.1. Menüben felhasznált betűtípus

A játékon kívül mindenhol, például a menüben is ugyanazt a betűtípust használtam, amit a 
következő linken lehet elérni: 
https://www.dafont.com/wash-your-hand.font?psize=s&text=Exit 

 

A betűtípus a következőképpen néz ki: 

<center>

 ![46](https://github.com/lacko186/Markdown_/blob/main/markdown/46.PNG)
 
 </center>
 
#### 3.5.2. Játékban felhasznált betűtípus

A játékon belülre egy olyan betűtípust szerettem volna használni, amely illik a 
pixelgrafikus környezetbe. A betűtípus linkje: 
https://www.dafont.com/press-start-2p.font 
A betűtípus kinézete: 

 

### 3.9. Tesztdokumentáció
---

<p>A program szinte tökéletesen működik, hibaüzenetekre alapból nincs rá szükség, mivel a 
gombokra kattintva válthat az ablakok között. A karakter mozgása néhol nem működik 
tökéletesen a fizikai határokkal, hogyha *collide* közben a játékos a vele ellentétes irányba 
mozogna úgy, hogy két ellentétes irányú billentyűt nyom le egyszerre és az egyiket hirtelen 
felengedi. 
A játék tesztelve lett több, informatikához szakmailag nem értő személyekkel, akiknek a játék 
tetszett, ám nehézségeik akadtak egy- egy ponton a játék fizikájával. Ezen felül pozitív 
visszajelzéseket kaptam a programomról. </p>

---

## 4. Fejlesztési lehetőségek

A játékomba több fejlesztési lehetőség is eszembe jutott: 

* A játékosnév megadásakor lehetne különböző kinézetű karakterek közül is 
választani 
* Nagyobb játéktér, több pálya, helyiség 
* Több NJK, valamint több küldetés 
* Többfajta küldetés 
* Alájátszási zenét lehetne rakni a játékba 
* A játék fizikájának szofisztikáltabb megvalósítás

---

## 5. Irodalomjegyzék

* https://www.pygame.org/docs/ 
* https://stackoverflow.com/ 
* https://www.dafont.com/ 
* https://pypi.org/project/auto-py-to-exe/ - exe konverter 
* https://www.google.com/search?q=pok%C3%A9mon+tileset&safe=strict&source=lnms&tbm=isch&sa=X&ved=2ahUKEwiGksSRwqLpAhV05aYKHX90ClsQ_AUoAXoECAsQAw&biw=1280&bih=586#imgrc=rKcOqlZhFS_gQM&imgdii=qdURQfY87oihIM – a játéktér kialakításában használt elemeket tartalmazó kép 
* https://techwithtim.net/tutorials/game-development-with-python/pygame-
tutorial/pygame-animation/ - az animáció és annak mozgásba bevitele 
* https://github.com/techwithtim/Tower-Defense-Game/blob/master/run.py - a run fájl 
használata 
* https://www.spriters-resource.com/ds_dsi/pokemonblack2white2/sheet/48049/ - az 
összes karakter alapját tartalmazó kép 
* https://stackoverflow.com/questions/46390231/how-to-create-a-text-input-box-with-
pygame - felhasználónév inputboxa és a gomb működése 

 

---
<button></button>
## 6. Elérhetőségek
 
Amennyiben problémája, esetleg javaslata lenne a programmal kapcsolatban, kérem a 
[rebmanfanny@gmail.com](rebmanfanny@gmail.com) email címen keressen meg. 

