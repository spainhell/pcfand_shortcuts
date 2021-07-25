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
        <h4>Kalkulačka</h4>
        <h4>Nápověda</h4>

        <h3>Aritmetické funkce</h3>

        <h3>Tisk textu</h3>
        <h4>Řídící klávesy</h4>
        <h4>Ovládání tiskárny</h4>
        <h4>Tečkové příkazy</h4>
        <h4>Typy písma</h4>

        <h3>Grafika</h3>
        <h4>Zobrazení</h4>
        <h4>Tisk, export</h4>

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