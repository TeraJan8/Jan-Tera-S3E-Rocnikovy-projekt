## Jan-Tera-ovládání-LED-pásku-pomocí-ESP8266
### Wi‑Fi ovládání LED pásku pomocí ESP8266

Cíl: Vytvořit ovládání LED pásku přes Wi‑Fi pomocí modulu ESP8266 NodeMCU V3, které umožní zapínat a vypínat pásek z telefonu a zároveň nabídne manuální ovládání tlačítkem. Projekt slouží k zjednodušení každodenního používání osvětlení a k procvičení pájení, práce s ESP a programování.

### Použité komponenty a jejich funkce

ESP8266 Lua NodeMCU V3 Funkce: hlavní řídicí jednotka; připojuje se k Wi‑Fi a běží na něm webserver pro ovládání LED pásku. Důvod volby: podporuje Wi‑Fi a snadné programování.

IRLZ44N MOSFET Tranzistor Funkce: spínací prvek pro LED pásek. ESP8266 dává řídicí signál 3,3 V, ale LED pásek běží na 12 V; MOSFET přepíná napájení 12 V podle signálu z ESP. Poznámka: používáme MOSFET, protože běžné GPIO z ESP nedokáže přímo napájet vysoký proud pro LED pásek.

Rezistor 220 Ω 0.6 W 1% 50 ppm Funkce: omezovací rezistor (např. pro ochranu LED indikace nebo brány MOSFETu při zapojení s LED diodami). Proč 0.6 W: vyšší výkonová rezerva zajišťuje, že rezistor se nepřehřívá při krátkodobém zatížení; 0.6 W je bezpečná volba pro malé obvody a zvyšuje spolehlivost.

Rezistor 100 kΩ 0.6 W 1% 50 ppm Funkce: pull‑down nebo pull‑up v obvodu tlačítka či pro stabilizaci vstupu; zajišťuje definovaný stav při uvolněném tlačítku.

Jednobarevný LED pásek cca 5 m Funkce: hlavní osvětlení, které upravím na přesnou délku a tvar podle stolu. Pásek budu stříhat podle dělicích míst a napájet v sekcích tak, aby seděl na tvar stolu.

Tlačítko Funkce: manuální přepínání stavu LED pásku; bude zabudované do plastové krabičky a připojené na PCB.

Plastová krabička a prototypová PCB Funkce: krabička schová elektroniku; PCB slouží k přehlednému a pevnějšímu propojení komponent.

Napájení ESP8266: micro‑USB kabel připojený k 5V adaptéru.

### Současný stav

Seznam součástek (aktuálně): ESP8266 NodeMCU V3 (IMG_1243.JPEG), Rezistor 220 Ω 0.6 W 1% 50 ppm (IMG_1242.JPEG), Rezistor 100 kΩ 0.6 W 1% 50 ppm (IMG_1242.JPEG), IRLZ44N MOSFET (IMG_1242.JPEG), LED pásek cca 5m (IMG_1244.JPEG), tlačítko a propojovací kabely (IMG_1249.JPEG).

Objednané položky: plastová krabička (Snímek obrazovky 2025-12-18 135821.jpg) a prototypová PCB deska Snímek obrazovky (2025-12-18 135903.jpg).

LED pásek je připraven k rozstříhání a napájení podle délky stolu.

Fotky komponentů jsou vyfoceny a jsou přiloženy v repozitáři.

### Plánované kroky

Přesné rozstříhání a napájení LED pásku podle tvaru stolu.

Sestavení obvodu na prototypové PCB a umístění do plastové krabičky.

Naprogramovat za pomocí AI kód, který bude vyhovovat mým požadavkům.

Nahrání a otestování kódu do ESP8266, ladění webového rozhraní.

Finalizace dokumentace a nahrání všech materiálů na GitHub.

### Zdroje

Seznam a výběr komponent byl konzultován a částečně vygenerován s pomocí AI asistenta Microsoft Copilot; návrh byl následně upraven a otestován autorem projektu.
