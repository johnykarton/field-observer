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
SloupecPopisidPořadové číslo bodutimestampČas záznamu v UTC (ISO 8601)lat / lonSouřadnice WGS-84alt_mNadmořská výška (m)acc_mPřesnost GPS (m)az_geo_degAzimut – geografický sever (0–360°, 1 desetinné místo)az_mag_degAzimut – magnetický sever (0–360°, 1 desetinné místo)decl_degMagnetická deklinace použitá pro výpočettilt_beta_degNáklon předo-zadní osa βtilt_gamma_degNáklon boční osa γnotePoznámka / ID fotky
