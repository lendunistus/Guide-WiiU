# Tiramisu

## Lage en NAND backup{docsify-ignore}

Hvis noe går galt senere i prosessen og Wii U konsollen "bricker", vil gjenoppretting av en NAND backup muligens fikse den.

### Instruksjoner {docsify-ignore}

?> Størrelsen på Wii U NAND er (avhengig av modellen) enten 8gb eller 32gb. På grunn av dette så må du bruke ett SD-kort som er større enn NAND størrelsen. Hvis SD-kortet ditt ikke er stort nok, så kan du hoppe over `MLC` delen hvor spilldata og saves er lagret, den er ikke nødvendig for å gjenopprette de fleste bricke-tilfellene.

?> Å gjenopprette en NAND backup på Wii U konsollen krever litt kunskap om maskinvare og loddeferdigheter av mikro elektronikk. <br>Men å lage en NAND backup er **alltid** lurt, så du burde ikke hoppe over det. <br>NAND backupen din er unik for ditt system. backups fra andre konsoller vil **ikke** fungere.

1. Launch web browser exploit as [previously explained](browser-exploit) but this time, you will need to hold the B button.
1. Navigate to `nanddumper` using the Gamepad and press A to launch it.
1. Bruk D-padden for å sette opp følgende konfigurasjon:
    - Dump SLC: **yes**
    - Dump SLCCMPT: **yes**
    - Dump MLC: **optional**
    - Dump OTP: **yes**
    - Dump SEEPROM: **yes**
1. Trykk på A knappen for å starte dumpingprosessen.
1. Når prosessen er fullført, skru av Wii U konsollen, ta ut SD-kortet og sett den inn i PC-en din.
1. For å forsikre deg om at du ikke mister filene, kopier `slc.bin`, `slccmpt.bin`, `seeprom.bin`, `otp. ` og hvis du valgte å gå for full sikkerhetskopi, `hver mlc.bin.part` til PC'en din.
1. Slett filene fra SD-kortet for å frigjøre plass.

?> **If the PayloadLoader is already installed into the Health and Safety Information app and your console is already autobooting it, you do not need to continue following the guide.**