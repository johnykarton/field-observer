# field-observer
Jednoduchá webová aplikace pro terénní dokumentaci pozorovacích bodů. Navržena pro použití na iPhonu v Safari – bez instalace, bez App Store.
K čemu to je
Při terénním průzkumu potřebuješ na jednom místě vidět:

kam přesně se díváš (azimut – geografický i magnetický)
jak je fotoaparát nakloněný (náklon β a γ)
kde stojíš (GPS)

Aplikace tato data sloučí do jednoho bodu, který si uložíš a exportuješ do CSV nebo GeoJSON pro další zpracování v QGIS.
Funkce

Geografický azimut (primární) + magnetický azimut s automatickou deklinací z NOAA
Vodováha – vizuální 2D bublina + hodnoty β (předo-zadní) a γ (boční náklon)
GPS – souřadnice, nadmořská výška, přesnost
Uložení bodu – snapshot všech hodnot + volitelná poznámka / ID fotky
Export – CSV a GeoJSON kompatibilní s QGIS / QField
Funguje jako PWA – lze přidat na plochu jako ikonu

Jak spustit
Otevři v Safari na iPhonu:
https://johnykarton.github.io/field-observer
Při prvním spuštění povol přístup k senzorům orientace. GPS se aktivuje automaticky.

⚠️ Používej Safari, ne Chrome. Chrome na iOS nemá přístup ke kompasu.

Struktura exportu (CSV)
id                Pořadové číslo bodu
timestamp         Čas záznamu v UTC (ISO 8601)
lat / lon         Souřadnice WGS-84
alt_m             Nadmořská výška (m)
acc_m             Přesnost GPS (m)
az_geo_deg        Azimut – geografický sever (0–360°, 1 desetinné místo)
az_mag_deg        Azimut – magnetický sever (0–360°, 1 desetinné místo)
decl_deg          Magnetická deklinace použitá pro výpočet
tilt_beta_deg     Náklon předo-zadní osa β
tilt_gamma_deg    Náklon boční osa γ
note              Poznámka / ID fotky
