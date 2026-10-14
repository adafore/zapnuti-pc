# Zapnutí PC

Minimalistický ovladač domácího PC: podržet Zapnout PC 2,5 sekundy nebo Vypnout PC 4 sekundy. Obyčejný klik nic neodesílá. Stránka nezjišťuje stav počítače; potvrzuje pouze odeslání povelu.

Statická stránka pro GitHub Pages, bez buildu a externích knihoven. Přístupový kód se zadává do nastavení. Skutečný kód není součástí tohoto repozitáře. Ukládání na zařízení je volitelné.

Povely se přes ntfy.sh podepisují pomocí HMAC-SHA-256, časového údaje a jednorázového UUID. Telefon s Termuxem zpracuje `on` a odešle Wake-on-LAN. Přijímač Windows zpracuje `off` a požádá o běžné vypnutí bez nuceného zavírání programů. Windows přijímač musí běžet; ve výchozím nastavení se spouští po přihlášení uživatele.

Tento repozitář obsahuje pouze web. Soukromé konfigurace, klíče a logy sem nepatří.
