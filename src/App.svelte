<script lang="ts">
	import Keyb from './Keyb.svelte';
	import Color from './Color.svelte';
</script>

<h1>PC FAND&reg</h1>
<h2>Referenční seznam funkčních kláves, příkazů a funkcí</h2>

<ul>
    <li>
        <h3>I. Uživatelská část</h3>

        <h3>Datový editor</h3>

        <h4>Pohyb po údajích</h4>
        <table>
            <tr><td><Keyb labels={["&larr;"]}/></td><td>předchozí údaj</td></tr>
            <tr><td><Keyb labels={["&rarr;"]}/></td><td>následující údaj</td></tr>
            <tr><td><Keyb labels={["Enter"]}/></td><td>další editovaný údaj</td></tr>
            <tr><td><Keyb labels={["Home"]}/></td><td>první údaj ve větě</td></tr>
            <tr><td><Keyb labels={["End"]}/></td><td>poslední pořízený údaj ve větě</td></tr>
            <tr><td><Keyb labels={["Ctrl", "&bsol;"]} delims={["+"]}/></td><td>na začátek další věty</td></tr>
        </table>

        <h4>Pohyb po větách</h4>
        <table>
            <tr><td><Keyb labels={["Page Up"]}/></td><td>o obrazovku vzad</td></tr>
            <tr><td><Keyb labels={["Page Down"]}/></td><td>o obrazovku vpřed</td></tr>
            <tr><td><Keyb labels={["&uarr;", "Ctrl", "Home"]} delims={[", ", "+"]}/></td><td>předchozí věta</td></tr>
            <tr><td><Keyb labels={["&darr;", "Ctrl", "End"]} delims={[", ", "+"]}/></td><td>následující věta</td></tr>
            <tr><td><Keyb labels={["Ctrl", "Page Up"]} delims={["+"]}/></td><td>první věta</td></tr>
            <tr><td><Keyb labels={["Ctrl", "Page Down"]} delims={["+"]}/></td><td>poslední věta</td></tr>
            <tr><td><Keyb labels={["F3"]}/></td><td>najdi větu (podle klíč. údaje)</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F3"]} delims={["+"]}/></td><td>najdi větu (podle jejího čísla)</td></tr>
        </table>

        <h4>Editace údajů</h4>
        <table>
            <tr><td><Keyb labels={["Insert"]}/></td><td>zahájení opravy údaje</td></tr>
            <tr><td><Keyb labels={["Insert", "Ctrl", "V"]} delims={[", ", "+"]}/></td><td>vkládání / přepis</td></tr>
            <tr><td><Keyb labels={["&larr;"]}/></td><td>o znak doleva</td></tr>
            <tr><td><Keyb labels={["&rarr;"]}/></td><td>o znak doprava</td></tr>
            <tr><td><Keyb labels={["Home"]}/></td><td>na začátek údaje</td></tr>
            <tr><td><Keyb labels={["End"]}/></td><td>na konec údaje</td></tr>
            <tr><td><Keyb labels={["Delete"]}/></td><td>výmaz znaku nad kurzorem</td></tr>
            <tr><td><Keyb labels={["Back space"]}/></td><td>výmaz znaku před kurzorem</td></tr>
            <tr><td><Keyb labels={["Enter"]}/></td><td>ukončení editace údaje</td></tr>
            <tr><td><Keyb labels={["Esc"]}/></td><td>-''-, ale bez provedení změn</td></tr>
            <tr><td><Keyb labels={["F4"]}/></td><td>doplň diakritické znaménko</td></tr>
            <tr><td><Keyb labels={["Alt", "F8"]} delims={["+"]}/></td><td>jiná klávesnice</td></tr>
        </table>

        <h4>Volné texty</h4>
        <table>
            <tr><td>'.'</td><td>prázdný text</td></tr>
            <tr><td>'*'</td><td>text obsahuje znaky</td></tr>
            <tr><td><Keyb labels={["Insert"]}/></td><td>editace</td></tr>
            <tr><td><Keyb labels={["Esc"]}/></td><td>ukončení editace</td></tr>
            <tr><td><Keyb labels={["Ctrl", "Home"]} delims={["+"]}/></td><td>předchozí volný text</td></tr>
            <tr><td><Keyb labels={["Ctrl", "End"]} delims={["+"]}/></td><td>následující volný text</td></tr>
        </table>

        <h4>Editace vět</h4>
        <table>
            <tr><td><Keyb labels={["F2"]}/></td><td>pořiď / edituj větu</td></tr>
            <tr><td><Keyb labels={["Ctrl", "Y"]} delims={["+"]}/></td><td>vymaž větu (vybranou podmnožinu)</td></tr>
            <tr><td><Keyb labels={["Ctrl", "N"]} delims={["+"]}/></td><td>vlož novou větu před aktuální</td></tr>
            <tr><td><Keyb labels={["Ctrl", "U"]} delims={["+"]}/></td><td>obnov obsah věty před změnou</td></tr>
            <tr><td><Keyb labels={["Ctrl", "&larr;"]} delims={["+"]}/></td><td>přesuň větu o jednu nahoru</td></tr>
            <tr><td><Keyb labels={["Ctrl", "&rarr;"]} delims={["+"]}/></td><td>přesuň větu o jednu dolů</td></tr>
            <tr><td><Keyb labels={["F4"]}/></td><td>duplikuj údaj (z přechozí věty)</td></tr>
            <tr><td><Keyb labels={["F9"]}/></td><td>ulož</td></tr>
            <tr><td><Keyb labels={["Esc"]}/></td><td>uložení a ukončení editace</td></tr>
        </table>

        <h4>Další klávesy</h4>
        <table>
            <tr><td><Keyb labels={["Ctrl", "F2"]} delims={["+"]}/></td><td>obnovení obrazovky</td></tr>
            <tr><td><Keyb labels={["F5"]}/></td><td>PŘEPÍNAČE vypni/zapni</td></tr>
            <tr><td>&nbsp;&nbsp;Podmnožina</td><td>výběr vět</td></tr>
            <tr><td>&nbsp;&nbsp;Duplikace</td><td>kopírování údaje</td></tr>
            <tr><td>&nbsp;&nbsp;Tabelátor</td><td>výběr údajů pro editaci</td></tr>
            <tr><td>&nbsp;&nbsp;Aditivní změny</td><td>vazby do nadřízených souborů</td></tr>
            <tr><td>&nbsp;&nbsp;Kontroly</td><td>kontroly zadaných hodnot</td></tr>
            <tr><td><Keyb labels={["F6"]}/></td><td>AKCE</td></tr>
            <tr><td>&nbsp;&nbsp;Opis</td><td>automatické tiskové sestavy</td></tr>
            <tr><td>&nbsp;&nbsp;Kontroly</td><td>provedení kontrol (od akt. kurzoru)</td></tr>
            <tr><td>&nbsp;&nbsp;Nová podmnožina</td><td>podmínka podmnožiny vět</td></tr>
            <tr><td>&nbsp;&nbsp;Graf</td><td>grafické zobrazení dat</td></tr>
            <tr><td>&nbsp;&nbsp;Třídit</td><td>setřídění souboru (neindexových)</td></tr>
        </table>

        <h4>Navigace po databázi</h4>
        <table>
            <tr><td><Keyb labels={["F7"]}/></td><td>navigace nahoru (nadřízený soubor)</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F7"]} delims={["+"]}/></td><td>navigace dolů (podřízený soubor)</td></tr>
            <tr><td><Keyb labels={["Alt", "F7"]} delims={["+"]}/></td><td>navigace po všech souborech</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F4"]} delims={["+"]}/></td><td>návrat s převzetím hodnoty údaje</td></tr>
            <tr><td><Keyb labels={["Shift", "F7"]} delims={["+"]}/></td><td>navigace nahoru s aut. převzetím</td></tr>
        </table>

        <h3>Textový editor</h3>
        <p>Pozn. Následující příkazy platí pro textový editor (vyvolaný z hl. menu PC FANDu) a editaci volného textu v datovém souboru.</p>

        <h4>Pohyb kurzoru po textu</h4>
        <table>
            <tr><td><Keyb labels={["&larr;"]}/></td><td>předchozí znak</td></tr>
            <tr><td><Keyb labels={["&rarr;"]}/></td><td>následující znak</td></tr>
            <tr><td><Keyb labels={["&uarr;"]}/></td><td>předchozí řádek</td></tr>
            <tr><td><Keyb labels={["&darr;"]}/></td><td>následující řádek</td></tr>
            <tr><td><Keyb labels={["Ctrl", "&larr;"]} delims={["+"]}/></td><td>předchozí slovo</td></tr>
            <tr><td><Keyb labels={["Ctrl", "&rarr;"]} delims={["+"]}/></td><td>následující slovo</td></tr>
            <tr><td><Keyb labels={["Home"]}/></td><td>začátek řádku</td></tr>
            <tr><td><Keyb labels={["End"]}/></td><td>konec řádku</td></tr>
            <tr><td><Keyb labels={["Page Up"]}/></td><td>o obrazovku vzad</td></tr>
            <tr><td><Keyb labels={["Page Down"]}/></td><td>o obrazovku vpřed</td></tr>
            <tr><td><Keyb labels={["Ctrl", "Page Up"]} delims={["+"]}/></td><td>začátek textu</td></tr>
            <tr><td><Keyb labels={["Ctrl", "Page Down"]} delims={["+"]}/></td><td>konec textu</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F3"]} delims={["+"]}/></td><td>zadaný řádek číslo ...</td></tr>
            <tr><td><Keyb labels={["Ctrl", "Q", "E"]} delims={["+"]}/></td><td>první řádek obrazovky</td></tr>
            <tr><td><Keyb labels={["Ctrl", "Q", "X"]} delims={["+"]}/></td><td>poslední řádek obrazovky</td></tr>
            <tr><td><Keyb labels={["Ctrl", "W"]} delims={["+"]}/></td><td>obrazovka o řádek dolů</td></tr>
            <tr><td><Keyb labels={["Ctrl", "Z"]} delims={["+"]}/></td><td>obrazovka o řádek nahoru</td></tr>
        </table>

        <h4>Editace textu</h4>
        <table>
            <tr><td><Keyb labels={["Enter"]}/></td><td>nový řádek / odstavec</td></tr>
            <tr><td><Keyb labels={["Delete"]}/></td><td>výmaz znaku na kurzorem</td></tr>
            <tr><td><Keyb labels={["Back space"]}/></td><td>výmaz znaku před kurzorem</td></tr>
            <tr><td><Keyb labels={["Ctrl", "T"]} delims={["+"]}/></td><td>výmaz slova</td></tr>
            <tr><td><Keyb labels={["Ctrl", "Y"]} delims={["+"]}/></td><td>výmaz řádku</td></tr>
            <tr><td><Keyb labels={["Ctrl", "Q", "Y"]} delims={["+"]}/></td><td>výmaz od kurzoru do konce řádku</td></tr>
            <tr><td><Keyb labels={["Ctrl", "U"]} delims={["+"]}/></td><td>obnovení původního stavu</td></tr>
            <tr><td><Keyb labels={["Ctrl", "Q", "L"]} delims={["+"]}/></td><td>obnovení řádku (jen editovaného)</td></tr>
            <tr><td><Keyb labels={["Alt", "="]} delims={["+"]}/></td><td>ukončení editace bez uložení změn</td></tr>
            <tr><td><Keyb labels={["F9"]}/></td><td>ulož změny</td></tr>
            <tr><td><Keyb labels={["Esc"]}/></td><td>ukončení editace s uložením změn</td></tr>
            <tr><td><Keyb labels={["Ctrl", "N"]} delims={["+"]}/></td><td>vlož řádek před kurzor</td></tr>
            <tr><td><Keyb labels={["Ctrl", "I"]} delims={["+"]}/></td><td>tabelátor</td></tr>
            <tr><td><Keyb labels={["Ctrl", "J"]} delims={["+"]}/></td><td>tabelace zprava</td></tr>
            <tr><td><Keyb labels={["Ctrl", "O", "C"]} delims={["+"]}/></td><td>vycentrování textu na řádku</td></tr>
            <tr><td><Keyb labels={["F4"]}/></td><td>doplň diakritické znaménko</td></tr>
        </table>

        <h4>Kreslení rámečků</h4>
        <table>
            <tr><td><Keyb labels={["Ctrl", "Q", "-"]} delims={["+"]}/></td><td>vycentrování textu na řádku</td></tr>
            <tr><td><Keyb labels={["Ctrl", "Q", "="]} delims={["+"]}/></td><td>vycentrování textu na řádku</td></tr>
            <tr><td><Keyb labels={["Ctrl", "Q", "/"]} delims={["+"]}/></td><td>vycentrování textu na řádku</td></tr>
        </table>
        <p>v průběhu kreslení lze použít</p>
        <table>
            <tr><td><Keyb labels={["&larr;", "&rarr;", "&uarr;", "&darr;"]} delims={[", ", ", ", ", "]}/></td><td>kreslení čáry</td></tr>
            <tr><td><Keyb labels={["-"]}/></td><td>přepni na jednoduchou čáru</td></tr>
            <tr><td><Keyb labels={["="]}/></td><td>přepni na dvojitou čáru</td></tr>
            <tr><td><Keyb labels={["/"]}/></td><td>přepni na mazání čáry</td></tr>
            <tr><td><Keyb labels={[" "]}/></td><td>přepni na posun kurzoru</td></tr>
            <tr><td><Keyb labels={["-"]}/></td><td>konec kreslení</td></tr>
        </table>
        <p>Pozn. Při kreslení rámečku v kódové stránce 852 nelze napojovat jednoduchou čáru na dvojitou a naopak.</p>

        <h4>Přepínače textového editoru</h4>
        <table>
            <tr><td><Keyb labels={["Insert"]}/></td><td>vkládání / přepisování znaků</td></tr>
            <tr><td><Keyb labels={["Ctrl", "O", "I"]} delims={["+"]}/></td><td>odsazení zleva</td></tr>
            <tr><td><Keyb labels={["Ctrl", "O", "W"]} delims={["+"]}/></td><td>automatické formátování</td></tr>
            <tr><td><Keyb labels={["Ctrl", "O", "J"]} delims={["+"]}/></td><td>zarovnání vpravo při formátování</td></tr>
            <tr><td><Keyb labels={["Alt", "F6"]} delims={["+"]}/></td><td>vyber jinou tiskárnu</td></tr>
            <tr><td><Keyb labels={["Alt", "F8"]} delims={["+"]}/></td><td>vyber jinou klávesnici</td></tr>
            <tr><td><Keyb labels={["Ctrl", "K", "N"]} delims={["+"]}/></td><td>sloupcový / běžný blok</td></tr>
        </table>

        <h4>Bloky textu</h4>
        <table>
            <tr><td><Keyb labels={["Ctrl", "K", "B", "F7"]} delims={["+", "", ", "]}/></td><td>začátek bloku</td></tr>
            <tr><td><Keyb labels={["Ctrl", "K", "K", "F8"]} delims={["+", "", ", "]}/></td><td>konec bloku</td></tr>
            <tr><td><Keyb labels={["Shift", "&larr;"]} delims={["+"]}/></td><td>posun začátku/konce bloku po znaku</td></tr>
            <tr><td><Keyb labels={["Shift", "Page Up"]} delims={["+"]}/></td><td>posun začátku/konce bloku o stránku vzad</td></tr>
            <tr><td><Keyb labels={["Shift", "Page Down"]} delims={["+"]}/></td><td>posun začátku/konce bloku o stránku vpřed</td></tr>
            <tr><td><Keyb labels={["Ctrl", "K", "C"]} delims={["+"]}/></td><td>kopie bloku</td></tr>
            <tr><td><Keyb labels={["Ctrl", "K", "V"]} delims={["+"]}/></td><td>přenesení bloku</td></tr>
            <tr><td><Keyb labels={["Ctrl", "K", "Y"]} delims={["+"]}/></td><td>výmaz bloku</td></tr>
            <tr><td><Keyb labels={["Ctrl", "K", "R"]} delims={["+"]}/></td><td>načtení textového souboru</td></tr>
            <tr><td><Keyb labels={["Ctrl", "K", "W"]} delims={["+"]}/></td><td>zápis bloku do textového souboru</td></tr>
            <tr><td><Keyb labels={["Ctrl", "K", "P"]} delims={["+"]}/></td><td>tisk bloku</td></tr>
            <tr><td><Keyb labels={["Ctrl", "K", "F"]} delims={["+"]}/></td><td>formátování bloku</td></tr>
            <tr><td><Keyb labels={["Ctrl", "K", "U"]} delims={["+"]}/></td><td>změna malých písmen na velká</td></tr>
            <tr><td><Keyb labels={["Ctrl", "K", "L"]} delims={["+"]}/></td><td>změna velkých písmen na malá</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F7"]} delims={["+"]}/></td><td>kopie bloku do Clipboardu</td></tr>
            <tr><td><Keyb labels={["Shift", "F7"]} delims={["+"]}/></td><td>kopie bloku z Clipboardu</td></tr>
        </table>
        <p>Pozn. Clipboard je pomocná paměť pro přenos textu</p>

        <h4>Formátování textu</h4>
        <table>
            <tr><td><Keyb labels={["Ctrl", "O", "L"]} delims={["+"]}/></td><td>nastav levý okraj</td></tr>
            <tr><td><Keyb labels={["Ctrl", "O", "R"]} delims={["+"]}/></td><td>nastav pravý okraj</td></tr>
            <tr><td><Keyb labels={["Ctrl", "O", "W"]} delims={["+"]}/></td><td>zapni / vypni automatické formátování</td></tr>
            <tr><td><Keyb labels={["Ctrl", "O", "I"]} delims={["+"]}/></td><td>zapni / vypni odsazení zleva</td></tr>
            <tr><td><Keyb labels={["Ctrl", "O", "J"]} delims={["+"]}/></td><td>zapni / vypni zarovnání vpravo</td></tr>
            <tr><td><Keyb labels={["Enter"]}/></td><td>konec řádku / odstavce (tvrdý řádek)</td></tr>
            <tr><td><Keyb labels={["Ctrl", "B"]} delims={["+"]}/></td><td>formátuj text do konce odstavce</td></tr>
            <tr><td><Keyb labels={["Ctrl", "K", "F"]} delims={["+"]}/></td><td>formátuj text v označeném bloku</td></tr>
        </table>

        <h4>Vyhledávání a nahrazování</h4>
        <table>
            <tr><td><Keyb labels={["Ctrl", "Q", "F"]} delims={["+"]}/></td><td>hledání řetězce v textu</td></tr>
            <tr><td><Keyb labels={["Ctrl", "Q", "A"]} delims={["+"]}/></td><td>hledání a nahrazení řetězce jiným řetězcem</td></tr>
            <tr><td><Keyb labels={["Ctrl", "L"]} delims={["+"]}/></td><td>pokračuj v hledání / nahrazení</td></tr>
            <tr><td colspan="2">Podmínky pro hledání:</td></tr>
            <tr><td>g</td><td>v celém úseku</td></tr>
            <tr><td>e</td><td>globálně</td></tr>
            <tr><td>w</td><td>hledat jen celá slova (ne složeniny)</td></tr>
            <tr><td>~</td><td>lexikálně (hrábě = HRABE)</td></tr>
            <tr><td>u</td><td>bez rozlišení malá / velká písmena</td></tr>
            <tr><td>l</td><td>hledat jen v označeném bloku</td></tr>
            <tr><td>n</td><td>nahradit bez předchozího dotazu</td></tr>
        </table>

        <h3>Datový a textový editor</h3>
        <p>Pozn. Společné příkazy, které lze použít v datovém i textovém editoru</p>
        <h4>Kalkulačka</h4>
        <table>
            <tr><td><Keyb labels={["Ctrl", "F5"]} delims={["+"]}/></td><td>vyvolání kalkulačky na posl. řádku</td></tr>
            <tr><td><Keyb labels={["Ctrl", "U"]} delims={["+"]}/></td><td>obnovení posledního výpočtu</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F4"]} delims={["+"]}/></td><td>přenos výsledku do údaje / textu</td></tr>
        </table>

        <h4>Nápověda</h4>
        <table>
            <tr><td><Keyb labels={["F1"]}/></td><td>vyvolání nápovědy</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F1"]} delims={["+"]}/></td><td>nápověda k aktuálnímu údaji</td></tr>
            <tr><td><Keyb labels={["Alt", "F10"]} delims={["+"]}/></td><td>posledně vyvolaná nápověda</td></tr>
            <tr><td colspan="2">při prohlížení lze použít:</td></tr>
            <tr><td><Keyb labels={["&larr;", "&rarr;", "&uarr;", "&darr;"]} delims={[", ", ", ", ", "]}/></td><td>pohyb po zvýrazněných heslech</td></tr>
            <tr><td><Keyb labels={["Enter"]}/></td><td>nápověda k aktuálnímu heslu</td></tr>
            <tr><td><Keyb labels={["F10"]}/></td><td>předchozí zobrazená nápověda</td></tr>
            <tr><td><Keyb labels={["F1"]}/></td><td>index nápovědy</td></tr>
            <tr><td><Keyb labels={["F6"]}/></td><td>tisk aktuální zobrazené nápovědy</td></tr>
            <tr><td><Keyb labels={["Esc"]}/></td><td>ukončení prohlížení nápovědy</td></tr>
            <tr><td><Keyb labels={["Page Up"]}/></td><td>o obrazovku vzad</td></tr>
            <tr><td><Keyb labels={["Page Down"]}/></td><td>o obrazovku vpřed</td></tr>
            <tr><td><Keyb labels={["Ctrl", "Home"]} delims={["+"]}/></td><td>přechod na předchozí heslo helpu</td></tr>
            <tr><td><Keyb labels={["Ctrl", "End"]} delims={["+"]}/></td><td>přechod na následující heslo helpu</td></tr>
        </table>

        <h3>Aritmetické funkce</h3>
        <table>
            <tr><td>abs(ČíselnýVýraz)</td><td>absolutní hodnota</td></tr>
            <tr><td>arctan(ČíselnýVýraz)</td><td>arcus tangens</td></tr>
            <tr><td>cos(ČíselnýVýraz)</td><td>cosinus</td></tr>
            <tr><td>exp(ČíselnýVýraz)</td><td>exponenciela</td></tr>
            <tr><td>frac(ČíselnýVýraz)</td><td>desetinná část čísla</td></tr>
            <tr><td>int(ČíselnýVýraz)</td><td>celá část čísla</td></tr>
            <tr><td>ln(ČíselnýVýraz)</td><td>přirozený logaritmus</td></tr>
            <tr><td>pi</td><td>Ludolfovo číslo (3.1415926536)</td></tr>
            <tr><td>sqr(ČíselnýVýraz)</td><td>druhá mocnina</td></tr>
            <tr><td>sqrt(ČíselnýVýraz)</td><td>druhá odmocnina</td></tr>
            <tr><td>sin(ČíselnýVýraz)</td><td>sinus</td></tr>
            <tr><td>random</td><td>generátor náhodných čísel &lt;0,1)</td></tr>
        </table>

        <h3>Tisk textu</h3>
        <p>Pozn. Následující příkazy jsou platné jen pro textový editor.</p>

        <h4>Řídící klávesy</h4>
        <table>
            <tr><td><Keyb labels={["F6"]}/></td><td>tisk celého textu</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F6"]} delims={["+"]}/></td><td>tisk od pozice kurzoru do konce t.</td></tr>
            <tr><td><Keyb labels={["Ctrl", "K", "P"]} delims={["+"]}/></td><td>tisk označeného bloku</td></tr>
            <tr><td><Keyb labels={["Alt", "F6"]} delims={["+"]}/></td><td>výběr jiné tiskárny</td></tr>
            <tr><td><Keyb labels={["Esc"]}/></td><td>přerušení tisku</td></tr>
        </table>

        <h4>Ovládání tiskárny</h4>
        <p>Pozn. Těmito kombinacemi kláves se vkládají znaky do textu v místě kde je požadována příslušná činnost. Toto je v textu odlišně značeno zvýrazněnými znaky.</p>
        <table>
            <tr><td><Keyb labels={["Ctrl", "P", "G"]} delims={["+"]}/></td><td>zvukové znamení</td></tr>
            <tr><td><Keyb labels={["Ctrl", "P", "H"]} delims={["+"]}/></td><td>zpět o 1 znak</td></tr>
            <tr><td><Keyb labels={["Ctrl", "P", "L"]} delims={["+"]}/></td><td>odstránkování</td></tr>
        </table>

        <h4>Tečkové příkazy</h4>
        <p>Pozn. Tato tzv. tečková notace musí být vždy na začátku tištěného textu a každá na samostatném řádku.</p>
        <table>
            <tr><td>.ti n</td><td>počet výtisků (implicitně 1 výtisk)</td></tr>
            <tr><td>.cp n</td><td>počet volných řádků na konci strany</td></tr>
            <tr><td>.pl n</td><td>délka stránky v řádcích (impl. 72)</td></tr>
            <tr><td>.po n</td><td>odsazení zleva (implicitně 0 znaků)</td></tr>
            <tr><td colspan="2">parametr n je číselná hodnota</td></tr>
            <tr><td>.ff</td><td>potlačení nastavení papíru a odstr.</td></tr>
            <tr><td>.nm</td><td>jako .ff, na konci ale odstránkuje</td></tr>
            <tr><td>.he text</td><td>hlavička každé strany</td></tr>
            <tr><td>.fo text</td><td>zakončení každé strany</td></tr>
            <tr><td colspan="2">parametr text může také obsahovat tyto masky:</td></tr>
            <tr><td>___</td><td>maska pro vložení čísla stránky</td></tr>
            <tr><td>__.__.__</td><td>maska pro vložení aktuál. datumu</td></tr>
            <tr><td>__:__</td><td>maska pro vložení aktuálního času</td></tr>
        </table>

        <h4>Typy písma</h4>
        <p>Pozn. Použití a funkce těchto typů písma jsou závislé na typu tiskárny, které se ovládá pomocí EscapeSekvencí nastavených v programu FANDINST.</p>
        <table>
            <tr><td><Keyb labels={["Ctrl", "P", "S"]} delims={["+"]}/></td><td>podtržené písmo</td></tr>
            <tr><td><Keyb labels={["Ctrl", "P", "W"]} delims={["+"]}/></td><td>kurzíva (italic - šikmé písmo)</td></tr>
            <tr><td><Keyb labels={["Ctrl", "P", "B"]} delims={["+"]}/></td><td>tučně (bold)</td></tr>
            <tr><td><Keyb labels={["Ctrl", "P", "D"]} delims={["+"]}/></td><td>dvojitě (double)</td></tr>
            <tr><td><Keyb labels={["Ctrl", "P", "Q"]} delims={["+"]}/></td><td>široký tisk (wide - dvojnásobná šířka)</td></tr>
            <tr><td><Keyb labels={["Ctrl", "P", "E"]} delims={["+"]}/></td><td>hustě (compressed 17 CPI)</td></tr>
            <tr><td><Keyb labels={["Ctrl", "P", "A"]} delims={["+"]}/></td><td>perlička (elite 12 CPI)</td></tr>
            <tr><td><Keyb labels={["Ctrl", "P", "X"]} delims={["+"]}/></td><td>vysoké znaky (dvojnásobná výška)</td></tr>
            <tr><td><Keyb labels={["Ctrl", "P", "V"]} delims={["+"]}/></td><td>čtyřnásobné písmo (výška i šířka)</td></tr>
            <tr><td><Keyb labels={["Ctrl", "P", "T"]} delims={["+"]}/></td><td>husté řádkování (8 LPI)</td></tr>
        </table>

        <h3>Grafika</h3>
        <h4>Zobrazení</h4>
        <table>
            <tr><td><Keyb labels={["F4"]}/></td><td>inverzní zobrazení obrazovky</td></tr>
            <tr><td><Keyb labels={["Shift", "F4"]} delims={["+"]}/></td><td>inverzní zobrazení aktuálního okna</td></tr>
            <tr><td><Keyb labels={["&larr;", "&rarr;", "&uarr;", "&darr;"]} delims={[", ", ", ", ", "]}/></td><td>pohyb obrázku v okně</td></tr>
            <tr><td><Keyb labels={["Ctrl", "&larr;"]} delims={["+"]}/></td><td>o okno vlevo</td></tr>
            <tr><td><Keyb labels={["Ctrl", "&rarr;"]} delims={["+"]}/></td><td>o okno vpravo</td></tr>
            <tr><td><Keyb labels={["Page Up"]}/></td><td>o obrazovku nahoru</td></tr>
            <tr><td><Keyb labels={["Page Down"]}/></td><td>o obrazovku dolů</td></tr>
            <tr><td><Keyb labels={["Esc"]}/></td><td>ukončení zobrazení</td></tr>
        </table>

        <h4>Tisk, export</h4>
        <table>
            <tr><td><Keyb labels={["F6"]}/></td><td>tisk obrazovky</td></tr>
            <tr><td><Keyb labels={["Shift", "F6"]} delims={["+"]}/></td><td>tisk aktuálního okna</td></tr>
            <tr><td><Keyb labels={["Esc"]}/></td><td>přerušení tisku</td></tr>
            <tr><td><Keyb labels={["F9"]}/></td><td>uložení obrazovky do souboru PCX</td></tr>
            <tr><td><Keyb labels={["Shift", "F9"]} delims={["+"]}/></td><td>uložení aktuálního okna do souboru</td></tr>
        </table>

        <h3>Operátory</h3>
        <h4>Logické operátory</h4>
        <table>
            <tr><td></td><td>^</td><td>Operand ... negace</td><td>ne</td></tr>
            <tr><td>Operand</td><td>&</td><td>Operand ... konjunkce</td><td>a současně</td></tr>
            <tr><td>Operand</td><td>|</td><td>Operand ... disjunkce</td><td>nebo</td></tr>
            <tr><td>Operand</td><td>=&gt;</td><td>Operand ... implikace</td><td>jestliže, pak</td></tr>
            <tr><td>Operand</td><td>&lt;=&gt;</td><td>Operand ... ekvivalence</td><td>právě když</td></tr>
        </table>

        <h4>Srovnávací operátory</h4>
        <table>
            <tr><td></td><td></td><td>Operátor.Číslo</td><td>srovnání na (Číslo) počet desetinných míst (impl. 5 míst)</td></tr>
            <tr><td></td><td></td><td>Operátor~</td><td>lexikální porovnání (e=é=ě=E=É=Ě, r=R&lt;ř=Ř)</td></tr>
            <tr><td>Operand</td><td>=</td><td>Operand</td><td>je rovno</td></tr>
            <tr><td>Operand</td><td>&lt;&gt;</td><td>Operand</td><td>není rovno</td></tr>
            <tr><td>Operand</td><td>&gt;</td><td>Operand</td><td>je větší</td></tr>
            <tr><td>Operand</td><td>&gt;=</td><td>Operand</td><td>je větší nebo rovno</td></tr>
            <tr><td>Operand</td><td>&lt;</td><td>Operand</td><td>je menší</td></tr>
            <tr><td>Operand</td><td>&lt;=</td><td>Operand</td><td>je menší nebo rovno</td></tr>
            <tr><td>Operand</td><td>in</td><td>[SeznamArgum.]</td><td>prvek množiny</td></tr>
        </table>

        <h4>Číselné operátory</h4>
        <table>
            <tr><td></td><td>-</td><td>Operand</td><td>unární mínus</td></tr>
            <tr><td>Operand</td><td>+</td><td>Operand</td><td>sčítání</td></tr>
            <tr><td>Operand</td><td>-</td><td>Operand</td><td>odčítání</td></tr>
            <tr><td>Operand</td><td>*</td><td>Operand</td><td>násobení</td></tr>
            <tr><td>Operand</td><td>/</td><td>Operand</td><td>dělení</td></tr>
            <tr><td>Operand</td><td>div</td><td>Operand</td><td>celočíselné dělení</td></tr>
            <tr><td>Operand</td><td>mod</td><td>Operand</td><td>celočíselný zbytek po dělení</td></tr>
            <tr><td>Operand</td><td>round</td><td>Operand</td><td>zaokrouhlení na počet míst daný druhým operandem</td></tr>
        </table>

        <h4>Textové operátory</h4>
        <table>
            <tr><td>Operand</td><td>+</td><td>Operand</td><td>zřetězení textu</td></tr>
        </table>

        <h4>Priorita operátorů</h4>
        <table>
            <tr><td>1.</td><td>unární</td><td>- ^</td></tr>
            <tr><td>2.</td><td>číselné multiplikativní</td><td>* / div mod</td></tr>
            <tr><td></td><td>číselné ostatní</td><td>round</td></tr>
            <tr><td>3.</td><td>číselné aditivní</td><td>+ -</td></tr>
            <tr><td></td><td>textové aditivní</td><td>+</td></tr>
            <tr><td>4.</td><td>srovnávací</td><td>= &lt;&gt; &gt; &gt;= &lt; &lt;=</td></tr>
            <tr><td>5.</td><td>logické multiplikativní</td><td>&amp;</td></tr>
            <tr><td>6.</td><td>aditivní</td><td>|</td></tr>
            <tr><td>7.</td><td>ostatní</td><td>=&gt; &lt;=&gt;</td></tr>
        </table>
    </li>

    <li>
        <h3>II. Programátorská část</h3>

        <h3>Projektantské prostředí</h3>
        <h4>Ladění a heslování</h4>
        <table>
            <tr><td><Keyb labels={["Ctrl", "F8"]} delims={["+"]}/></td><td>syntaktická kontrola úlohy</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F9"]} delims={["+"]}/></td><td>kontrola a spuštění jedné kapitoly</td></tr>
            <tr><td><Keyb labels={["Alt", "F9"]} delims={["+"]}/></td><td>spuštění úlohy kapitolou MAIN</td></tr>
            <tr><td><Keyb labels={["Shift", "F1"]} delims={["+"]}/></td><td>navigace po projektu</td></tr>
            <tr><td><Keyb labels={["F10"]}/></td><td>návrat z navigace</td></tr>
            <tr><td><Keyb labels={["Alt", "F3"]} delims={["+"]}/></td><td>editace katalogu úlohy</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F10"]} delims={["+"]}/></td><td>odladění (zaheslení) úlohy</td></tr>
            <tr><td colspan="2">Odpověď na dotaz - Chcete úlohu zaheslovat (A/N)?</td></tr>
            <tr><td>A</td><td>odladit a nenávratně zaheslovat</td></tr>
            <tr><td>N</td><td>pouze odladit</td></tr>
            <tr><td><Keyb labels={["Alt", "F10"]} delims={["+"]}/></td><td>odladit a nenávratně zaheslovat</td></tr>
        </table>

        <h4>Nápověda</h4>
        <table>
            <tr><td><Keyb labels={["Alt", "F1"]} delims={["+"]}/></td><td>nápověda k syntaxi kapitoly</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F1"]} delims={["+"]}/></td><td>nápověda k syntaxi klíčového slova</td></tr>
            <tr><td><Keyb labels={["Alt", "F10"]} delims={["+"]}/></td><td>poslední vyvolaná nápověda</td></tr>
            <tr><td><Keyb labels={["Alt", "F2"]} delims={["+"]}/></td><td>vyvolání editace nápovědy úlohy</td></tr>
            <tr><td>z úlohy</td><td>editace help-souboru</td></tr>
            <tr><td>z dat. souboru</td><td>editace nápovědy k údaji</td></tr>
            <tr><td>z menu</td><td>editace nápovědy k položce menu</td></tr>
            <tr><td colspan="2">Pozn. Při neexistenci hesla je věta spříslušným heslem automaticky doplněna.</td></tr>
            <tr><td><Keyb labels={["F3"]}/></td><td>hledání názvu při editaci helpu</td></tr>
            <tr><td><Keyb labels={["Ctrl", "Home"]} delims={["+"]}/></td><td>předchozí věta help-souboru</td></tr>
            <tr><td><Keyb labels={["Ctrl", "End"]} delims={["+"]}/></td><td>následující věta help-souboru</td></tr>
            <tr><td><Keyb labels={["F6"]}/></td><td>tisk aktuální zobrazené nápovědy</td></tr>
        </table>

        <h4>Další</h4>
        <table>
            <tr><td><Keyb labels={["Ctrl", "&larr;"]} delims={["+"]}/></td><td>přesun kapitoly nahoru</td></tr>
            <tr><td><Keyb labels={["Ctrl", "&rarr;"]} delims={["+"]}/></td><td>přesun kapitoly dolů</td></tr>
            <tr><td><Keyb labels={["F6"]}/></td><td>výpis zdrojového textu úlohy (tisk)</td></tr>
            <tr><td colspan="2">Další použitelné kombinace kláves jsou stejné jako u textového editoru, tj. práce s bloky, hledání, nahrazování atd.</td></tr>
        </table>

        <h3>Kódy řídících a funčních kláves</h3>
        <p>Pozn. Použít tyto kódy lze ve spojitosti s funkcí SetKeyBuf();</p>
        <h4>Bez prefixu '\0'</h4>
        <table>
            <tr>
                <td><Keyb labels={["Enter"]}/></td><td>\13</td>
                <td><Keyb labels={["Tab"]}/></td><td>\9</td>
            </tr>
            <tr><td><Keyb labels={["Esc"]}/></td><td>\27</td><td></td><td></td></tr>
            <tr><td><Keyb labels={["Ctrl", "P", "A"]} delims={["+"]}/> - <Keyb labels={["Ctrl", "P", "Z"]} delims={["+"]}/></td><td>\1 - \26</td><td></td><td></td></tr>
        </table>

        <h4>S prefixem '\0'</h4>
        <table>
            <tr><td><Keyb labels={["Insert"]}/></td><td>\0\82</td>
                <td><Keyb labels={["Ctrl", "="]} delims={["+"]}/></td><td>\0\131</td></tr>
            <tr><td><Keyb labels={["Delete"]}/></td><td>\0\83</td>
                <td><Keyb labels={["Ctrl", "Tab"]} delims={["+"]}/></td><td>\0\15</td></tr>
            <tr><td><Keyb labels={["Home"]}/></td><td>\0\71</td>
                <td><Keyb labels={["Ctrl", "Home"]} delims={["+"]}/></td><td>\0\119</td></tr>
            <tr><td><Keyb labels={["End"]}/></td><td>\0\79</td>
                <td><Keyb labels={["Ctrl", "End"]} delims={["+"]}/></td><td>\0\117</td></tr>
            <tr><td><Keyb labels={["Page Up"]}/></td><td>\0\73</td>
                <td><Keyb labels={["Ctrl", "Page Up"]} delims={["+"]}/></td><td>\0\132</td></tr>
            <tr><td><Keyb labels={["Page Down"]}/></td><td>\0\81</td>
                <td><Keyb labels={["Ctrl", "Page Down"]} delims={["+"]}/></td><td>\0\118</td></tr>
            <tr><td><Keyb labels={["&larr;"]}/></td><td>\0\75</td>
                <td><Keyb labels={["Ctrl", "&larr;"]} delims={["+"]}/></td><td>\0\115</td></tr>
            <tr><td><Keyb labels={["&rarr;"]}/></td><td>\0\77</td>
                <td><Keyb labels={["Shift", "&rarr;"]} delims={["+"]}/></td><td>\0\116</td></tr>
            <tr><td><Keyb labels={["&uarr;"]}/></td><td>\0\72</td>
                <td><Keyb labels={["&darr;"]}/></td><td>\0\80</td></tr>
            <tr><td></td></tr>
            <tr><td><Keyb labels={["F1"]}/></td><td>\0\59</td>
                <td><Keyb labels={["Shift", "F1"]} delims={["+"]}/></td><td>\0\84</td></tr>
            <tr><td><Keyb labels={["F2"]}/></td><td>\0\60</td>
                <td><Keyb labels={["Shift", "F2"]} delims={["+"]}/></td><td>\0\85</td></tr>
            <tr><td><Keyb labels={["F3"]}/></td><td>\0\61</td>
                <td><Keyb labels={["Shift", "F3"]} delims={["+"]}/></td><td>\0\86</td></tr>
            <tr><td><Keyb labels={["F4"]}/></td><td>\0\62</td>
                <td><Keyb labels={["Shift", "F4"]} delims={["+"]}/></td><td>\0\87</td></tr>
            <tr><td><Keyb labels={["F5"]}/></td><td>\0\63</td>
                <td><Keyb labels={["Shift", "F5"]} delims={["+"]}/></td><td>\0\88</td></tr>
            <tr><td><Keyb labels={["F6"]}/></td><td>\0\64</td>
                <td><Keyb labels={["Shift", "F6"]} delims={["+"]}/></td><td>\0\89</td></tr>
            <tr><td><Keyb labels={["F7"]}/></td><td>\0\65</td>
                <td><Keyb labels={["Shift", "F7"]} delims={["+"]}/></td><td>\0\90</td></tr>
            <tr><td><Keyb labels={["F8"]}/></td><td>\0\66</td>
                <td><Keyb labels={["Shift", "F8"]} delims={["+"]}/></td><td>\0\91</td></tr>
            <tr><td><Keyb labels={["F9"]}/></td><td>\0\67</td>
                <td><Keyb labels={["Shift", "F9"]} delims={["+"]}/></td><td>\0\92</td></tr>
            <tr><td><Keyb labels={["F10"]}/></td><td>\0\68</td>
                <td><Keyb labels={["Shift", "F10"]} delims={["+"]}/></td><td>\0\93</td></tr>
            <tr><td></td></tr>
            <tr><td><Keyb labels={["Ctrl", "F1"]} delims={["+"]}/></td><td>\0\94</td>
                <td><Keyb labels={["Alt", "F1"]} delims={["+"]}/></td><td>\0\104</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F2"]} delims={["+"]}/></td><td>\0\95</td>
                <td><Keyb labels={["Alt", "F2"]} delims={["+"]}/></td><td>\0\105</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F3"]} delims={["+"]}/></td><td>\0\96</td>
                <td><Keyb labels={["Alt", "F3"]} delims={["+"]}/></td><td>\0\106</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F4"]} delims={["+"]}/></td><td>\0\97</td>
                <td><Keyb labels={["Alt", "F4"]} delims={["+"]}/></td><td>\0\107</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F5"]} delims={["+"]}/></td><td>\0\98</td>
                <td><Keyb labels={["Alt", "F5"]} delims={["+"]}/></td><td>\0\108</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F6"]} delims={["+"]}/></td><td>\0\99</td>
                <td><Keyb labels={["Alt", "F6"]} delims={["+"]}/></td><td>\0\109</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F7"]} delims={["+"]}/></td><td>\0\100</td>
                <td><Keyb labels={["Alt", "F7"]} delims={["+"]}/></td><td>\0\110</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F8"]} delims={["+"]}/></td><td>\0\101</td>
                <td><Keyb labels={["Alt", "F8"]} delims={["+"]}/></td><td>\0\111</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F9"]} delims={["+"]}/></td><td>\0\102</td>
                <td><Keyb labels={["Alt", "F9"]} delims={["+"]}/></td><td>\0\112</td></tr>
            <tr><td><Keyb labels={["Ctrl", "F10"]} delims={["+"]}/></td><td>\0\103</td>
                <td><Keyb labels={["Alt", "F10"]} delims={["+"]}/></td><td>\0\113</td></tr>
        </table>

        <h3>Módy datového editoru</h3>
        <table>
            <tr><td>!!</td><td>editace pouze údajů dle parametru tab=, pokud není nastaven tab, nelze rušit a vkládat věty</td></tr>
            <tr><td>^y</td><td>je zakázano zrušení vět</td></tr>
            <tr><td>?y</td><td>před zrušením věty je vydán dotaz na potvrzení</td></tr>
            <tr><td>^n</td><td>zákaz vytváření nových vět</td></tr>
            <tr><td>F2</td><td>pořízení nových vět za koncem souboru a editace pouze těchto vět, mode='F2!!' - zákaz změn již pořízených vět</td></tr>
            <tr><td>01</td><td>editace pouze jedné věty, mode='01F2' - pořízení pouze jedné věty</td></tr>
            <tr><td>F3</td><td>hledání podle klíče, pokud věta dle zadaného klíče neexistuje, přepne se do režimu pořízení, po stisku <Keyb labels={["Esc"]}/> se hledání opakuje</td></tr>
            <tr><td>LI</td><td>při hledání věty pomocí <Keyb labels={["F3"]}/> je pro údaje typu A a N kurzor aktuálně nastaven již v průběhu zadávání hodnoty klíče</td></tr>
            <tr><td>&lt;=</td><td>potlačení hlášení "věta neexistuje" při hledání <Keyb labels={["F3"]}/></td></tr>
            <tr><td>#A</td><td>zákaz vypnutí aditivních změn uživatelem</td></tr>
            <tr><td>#L</td><td>zákaz vypnutí logických kontrol uživatelem</td></tr>
            <tr><td>??</td><td>ukončení editoru bez dotazu, při mode='01??' i bez stisku <Keyb labels={["Esc"]}/></td></tr>
            <tr><td>?e</td><td>vyžádá dotaz na ukončení při <Keyb labels={["Esc"]}/> (opak mode='??')</td></tr>
            <tr><td>F1</td><td>krátká nápověda na posledním řádku obrazovky k aktuálnímu údaji, pokud heslo existuje v help-souboru, pomocí <Keyb labels={["Ctrl", "F8"]} delims={["+"]}/> se vyvolá nápověda přes celou obrazovku</td></tr>
            <tr><td>F124</td><td>jako F1, ale na předposledním řádku obrazovky</td></tr>
            <tr><td>CO</td><td>jen v kombinaci s cond=(...), podmínka cond je pouze výběr podmnožiny, nebude kontrolována při aktualizaci (pořízení)</td></tr>
            <tr><td>^m</td><td>dvojitý klik levé klávesy myši přepnut z <Keyb labels={["Insert"]}/> na <Keyb labels={["Enter"]}/> (neplatí při editaci údaje)</td></tr>
            <tr><td>-&gt;</td><td>klávesy <Keyb labels={["&uarr;"]}/> a <Keyb labels={["&darr;"]}/> se chovají stejně jako <Keyb labels={["&larr;"]}/> a <Keyb labels={["&rarr;"]}/>, tj. pohyb po údajích</td></tr>
            <tr><td>r2</td><td>na druhý řádek obrazovky je vypsán výraz výběru podmnožiny (standardně se nevypisuje)</td></tr>
            <tr><td>EX</td><td>exit-procedury vyvolané klávesou lze vyvolat i z editace údaje typu T</td></tr>
            <tr><td>WX</td><td>pokud není určena podmnožina (cond, owner) u sdíleného indexového souboru, vytvoří se pracovní index umožňující ostatním účastníkům rušit věty (pouze LAN)</td></tr>
        </table>

        <h3>Kód přerušení (EDBREAK)</h3>
        <h4>Ukončení, exit událostí</h4>
        <table>
            <tr><td>0</td><td>ukončení <Keyb labels={["Esc"]}/></td></tr>
            <tr><td>11</td><td>při překročení času - watch (LAN)</td></tr>
            <tr><td>12</td><td>přerušení přechodem přes údaj (seznam údajů)</td></tr>
            <tr><td>13</td><td>při prázdné podmnožině a <b>mode='^n'</b></td></tr>
            <tr><td>14</td><td>z vložené editace <Keyb labels={["Ctrl", "F4"]} delims={["+"]}/></td></tr>
            <tr><td>15</td><td>ukončení <Keyb labels={["Esc"]}/> při blokování (LAN)</td></tr>
            <tr><td>16</td><td>nová věta nebo změna <b>exit=(...:RECORD)</b></td></tr>
            <tr><td>17</td><td>zrušení věty <Keyb labels={["Ctrl", "Y"]} delims={["+"]}/></td></tr>
        </table>

        <h4>Ukončení, exit funkčními klávesami</h4>
        <table>
            <tr><td>1 &divide; 10</td><td><Keyb labels={["Shift", "F1"]} delims={["+"]}/> až <Keyb labels={["Shift", "F10"]} delims={["+"]}/></td></tr>
            <tr><td>21 &divide; 30</td><td><Keyb labels={["F1"]}/> až <Keyb labels={["F10"]}/></td></tr>
            <tr><td>31 &divide; 40</td><td><Keyb labels={["Ctrl", "F1"]} delims={["+"]}/> až <Keyb labels={["Ctrl", "F10"]} delims={["+"]}/></td></tr>
            <tr><td>41 &divide; 50</td><td><Keyb labels={["Alt", "F1"]} delims={["+"]}/> až <Keyb labels={["Alt", "F10"]} delims={["+"]}/></td></tr>
        </table>

        <h4>Ukončení, exit kurzorovými klávesami</h4>
        <table>
            <tr><td>77</td><td><Keyb labels={["Tab"]}/></td><td>78</td><td><Keyb labels={["Ctrl", "Tab"]} delims={["+"]}/></td></tr>
            <tr><td>51</td><td><Keyb labels={["Home"]}/></td><td>75</td><td><Keyb labels={["Ctrl", "Home"]} delims={["+"]}/></td></tr>
            <tr><td>59</td><td><Keyb labels={["End"]}/></td><td>73</td><td><Keyb labels={["Ctrl", "End"]} delims={["+"]}/></td></tr>
            <tr><td>53</td><td><Keyb labels={["Page Up"]}/></td><td>76</td><td><Keyb labels={["Ctrl", "Page Up"]} delims={["+"]}/></td></tr>
            <tr><td>61</td><td><Keyb labels={["Page Down"]}/></td><td>74</td><td><Keyb labels={["Ctrl", "Page Down"]} delims={["+"]}/></td></tr>
            <tr><td>55</td><td><Keyb labels={["&larr;"]}/></td><td>71</td><td><Keyb labels={["Ctrl", "&larr;"]} delims={["+"]}/></td></tr>
            <tr><td>57</td><td><Keyb labels={["&rarr;"]}/></td><td>72</td><td><Keyb labels={["Ctrl", "&rarr;"]} delims={["+"]}/></td></tr>
            <tr><td>52</td><td><Keyb labels={["&uarr;"]}/></td><td>60</td><td><Keyb labels={["&darr;"]}/></td></tr>
            <tr><td>62</td><td><Keyb labels={["Insert"]}/></td></tr>
        </table>

        <h3>Tabulky Znaků</h3>
        Kódová stránka 1. část - společná<br>
        Kódová stránka č. 437 IBM - 2. část<br>
        Kódová stránka Kamenických - 2. část<br>
        Kódová stránka LATIN II - 2. část<br>

        <h3>Kódy barev</h3>
        <table>
            <tr>
                <th>text pozadí</th>
                <th>černý<br>zv.jas</th>
                <th>modrý<br>zv.jas</th>
                <th>zelený<br>zv.jas</th>
                <th>cyan<br>zv.jas</th>
                <th>červený<br>zv.jas</th>
                <th>fialový<br>zv.jas</th>
                <th>hnědý<br>zv.jas</th>
                <th>šedý<br>zv.jas</th>
            </tr>
            <tr>
                <td>černé</td>
                <td><Color colors={["000", "008"]}/></td>
                <td><Color colors={["001", "009"]}/></td>
                <td><Color colors={["002", "010"]}/></td>
                <td><Color colors={["003", "011"]}/></td>
                <td><Color colors={["004", "012"]}/></td>
                <td><Color colors={["005", "013"]}/></td>
                <td><Color colors={["006", "014"]}/></td>
                <td><Color colors={["007", "015"]}/></td>
            </tr>
            <tr>
                <td>modré</td>
                <td><Color colors={["016", "024"]}/></td>
                <td><Color colors={["017", "025"]}/></td>
                <td><Color colors={["018", "026"]}/></td>
                <td><Color colors={["019", "027"]}/></td>
                <td><Color colors={["020", "028"]}/></td>
                <td><Color colors={["021", "029"]}/></td>
                <td><Color colors={["022", "030"]}/></td>
                <td><Color colors={["023", "031"]}/></td>
            </tr>
            <tr>
                <td>zelené</td>
                <td><Color colors={["032", "040"]}/></td>
                <td><Color colors={["033", "041"]}/></td>
                <td><Color colors={["034", "042"]}/></td>
                <td><Color colors={["035", "043"]}/></td>
                <td><Color colors={["036", "044"]}/></td>
                <td><Color colors={["037", "045"]}/></td>
                <td><Color colors={["038", "046"]}/></td>
                <td><Color colors={["039", "047"]}/></td>
            </tr>
            <tr>
                <td>cyan</td>
                <td><Color colors={["048", "056"]}/></td>
                <td><Color colors={["049", "057"]}/></td>
                <td><Color colors={["050", "058"]}/></td>
                <td><Color colors={["051", "059"]}/></td>
                <td><Color colors={["052", "060"]}/></td>
                <td><Color colors={["053", "061"]}/></td>
                <td><Color colors={["054", "062"]}/></td>
                <td><Color colors={["055", "063"]}/></td>
            </tr>
            <tr>
                <td>červené</td>
                <td><Color colors={["064", "072"]}/></td>
                <td><Color colors={["065", "073"]}/></td>
                <td><Color colors={["066", "074"]}/></td>
                <td><Color colors={["067", "075"]}/></td>
                <td><Color colors={["068", "076"]}/></td>
                <td><Color colors={["069", "077"]}/></td>
                <td><Color colors={["070", "078"]}/></td>
                <td><Color colors={["071", "079"]}/></td>
            </tr>
            <tr>
                <td>fialové</td>
                <td><Color colors={["080", "088"]}/></td>
                <td><Color colors={["081", "089"]}/></td>
                <td><Color colors={["082", "090"]}/></td>
                <td><Color colors={["083", "091"]}/></td>
                <td><Color colors={["084", "092"]}/></td>
                <td><Color colors={["085", "093"]}/></td>
                <td><Color colors={["086", "094"]}/></td>
                <td><Color colors={["087", "095"]}/></td>
            </tr>
            <tr>
                <td>hnědé</td>
                <td><Color colors={["096", "104"]}/></td>
                <td><Color colors={["097", "105"]}/></td>
                <td><Color colors={["098", "106"]}/></td>
                <td><Color colors={["099", "107"]}/></td>
                <td><Color colors={["100", "108"]}/></td>
                <td><Color colors={["101", "109"]}/></td>
                <td><Color colors={["102", "110"]}/></td>
                <td><Color colors={["103", "111"]}/></td>
            </tr>
            <tr>
                <td>šedé</td>
                <td><Color colors={["112", "120"]}/></td>
                <td><Color colors={["113", "121"]}/></td>
                <td><Color colors={["114", "122"]}/></td>
                <td><Color colors={["115", "123"]}/></td>
                <td><Color colors={["116", "124"]}/></td>
                <td><Color colors={["117", "125"]}/></td>
                <td><Color colors={["118", "126"]}/></td>
                <td><Color colors={["119", "127"]}/></td>
            </tr>
        </table>
    </li>
</ul>


<style>
	table, th, td {
		border: solid grey 1px;
        border-collapse: collapse;
	}

	h1, h2, h3, h4 {
		/*color: #ff3e00;*/
		text-transform: uppercase;
		/*font-size: 4em;*/
		/*font-weight: 100;*/
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>