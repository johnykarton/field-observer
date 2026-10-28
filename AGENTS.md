# Pokyny pro agenty

Tato pravidla platí pro dlouhé úlohy v tomto repozitáři. Aktuální přímé instrukce uživatele mají přednost.

## Průběžný checkpoint pro dlouhé úlohy

- U vícekrokové úlohy, která může přesáhnout jednu relaci, založ nebo načti trvalý `WORK_STATE.md` v pracovním prostoru / pracovní větvi **před** významnými změnami. Při více souběžných úlohách používej vlastní podadresář, aby nedošlo k přepsání stavu jiné úlohy.
- Zaznamenej cíl a kritéria dokončení, ověřené hotové kroky, nehotové kroky, změněné soubory, větev a commit SHA, testy (prošlo/neprošlo/neprovedeno), závislosti služeb, blokátory a **přesný bezpečný další krok**.
- Aktualizuj po významném ověřeném milníku, nejpozději po pěti významných operacích, před dlouhou či rizikovou operací a před ukončením relace. Pokud máš důvěryhodný údaj o zbývající kapacitě Worku a klesne na 10 % nebo méně, checkpointuj okamžitě. Neodhaduj limit podle tokenů ani času.
- Zajisti přežití nové relace: v dočasném prostředí ulož checkpoint do schváleného trvalého úložiště (např. aktuální pracovní větev či projektová poznámka). Nepředpokládej, že necommitnutý soubor v dočasném stroji zůstane dostupný.
- Při obnově přečti checkpoint, samostatně ověř Git stav, aktuální soubory, služby a testy. Neopakuj potenciálně nevratnou operaci bez kontroly skutečného výsledku.
- Neukládej hesla, tokeny, citlivá osobní data ani surové důvěrné logy. Checkpointování nesmí obejít dohodnutý proces review nebo nasazování.
