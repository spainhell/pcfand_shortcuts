<script lang="ts">
	import Keyb from './Keyb.svelte';
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
        <h4>Srovnávací operátory</h4>
        <h4>Číselné operátory</h4>
        <h4>Textové operátory</h4>
        <h4>Priorita operátorů</h4>

    </li>

    <li>
        <h3>II. Programátorská část</h3>

        <h3>Projektantské prostředí</h3>
        <h4>Ladění a heslování</h4>
        <h4>Nápověda</h4>
        <h4>Další</h4>

        <h3>Kódy řídících a funčních kláves</h3>
        <h4>Bez prefixu '\0'</h4>
        <h4>S prefixem '\0'</h4>

        <h3>Módy datového editoru</h3>

        <h3>Kód přerušení</h3>
        <h4>Ukončení, exit událostí</h4>
        <h4>Ukončení, exit funkčními klávesami</h4>
        <h4>Ukončení, exit kurzorovými klávesami</h4>

        <h3>Tabulky Znaků</h3>
        Kódová stránka 1. část - společná<br>
        Kódová stránka č. 437 IBM - 2. část<br>
        Kódová stránka Kamenických - 2. část<br>
        Kódová stránka LATIN II - 2. část<br>

        <h3>Kódy barev</h3>
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