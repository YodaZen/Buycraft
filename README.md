# Buycraft til Superawesome servere!

Dette er et specielt desginet Buycraft, lavet med henblik på at gøre det bruger venligt!

For at kunne benytte dette skal du have følgende plugins:

**Skript 2.6.4 (Anvend venligst en fork til 1.8)**

**Skript-Yaml 1.4.1**

**SkBee 1.10.2**

`Bemærk: Skriptet er kun blevet testet til version 1.8.8`

# Kommandoer:

Skriptet inkluderer selvfølgelig standardkommandoen /buycraft med alias /buy, men derudover tilbyder vi også en særlig administrator buycraft-kommando!

Ved at have tilladelsen `buycraft.manage` kan du bruge kommandoen /buy info, som giver dig adgang til en bred vifte af kommandoer!

Med denne kommando kan du for eksempel tildele Shards (valuta) ved hjælp af /buy give <spiller> <antal>, få adgang til købshistorik og meget mere...

Vi stræber efter at levere en omfattende kommandopakke, der giver dig fuld kontrol over dine købsprocesser og forbedrer din administrative oplevelse på serveren. Kh ChatGPT <3


# Konfiguration
Skriptet er yderst konfigurerbart, hvilket giver dig fuld frihed til at tilpasse Buycraft-systemet efter dine egne ønsker og behov.

Vi har udviklet Skriptet med tanke på, at du kan tilføje så mange kategorier, underkategorier osv. som du måtte ønske! Alt dette opnås ganske enkelt ved at følge det angivne YML-mønster (YAML).

For eksempel er Ranks: en kategori, hvor Rank1: repræsenterer et produkt.

Derudover kan du tildele forskellige produkter en prioritet (priority), hvilket betyder, at hvis en spiller køber et produkt med f.eks. Priority 2, vil de ikke kunne købe et andet produkt fra samme kategori med en lavere prioritet.
(Dette kan dog undlades, hvis man gerne vil have, at de kan købe alle produkter)

Konfigurationsfilen, config.yml, kan findes ved følgende sti: _plugins/Skript/YAML/Buycraft/config.yml_

Vi håber, at vores Buycraft tilbyder dig en enestående mulighed for at udvide og tilpasse dit serverens købeprocess på bedst mulig vis.
```
Menues:
    Forside:
        Title: Buycraft
        Rows: 5
        Items:
            '1':
                Title: ' '
                Item: light blue glass pane
                Slots:
                - 0
                - 1
                - 2
                - 3
                - 4
                - 5
                - 6
                - 7
                - 8
                Settings:
                    ClickAction:
                    - '[CLOSE]'
            '2':
                Title: ' '
                Item: white glass pane
                Settings:
                    ClickAction:
                    - '[CLOSE]'
                Slots:
                - 36
                - 37
                - 38
                - 39
                - 40
                - 41
                - 42
                - 43
                - 44
            '3':
                Item: player head
                Value: eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvN2UyZWI0NzUxZTNjNTBkNTBmZjE2MzUyNTc2NjYzZDhmZWRmZTNlMDRiMmYwYjhhMmFhODAzYjQxOTM2M2NhMSJ9fX0=
                Slots:
                - 24
                Title: "&b&lTerms of Service&f&l:"
                Lore:
                - "&f- &7Klik for at åbne!"
                Settings:
                    ClickAction:
                    - '[PLAYSOUND] ORB_PICKUP'
                    - '[OPEN] TOS'
            '4':
                Item: player head
                Value: eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvZTIwNjQwMzZiMjMyYmVkNGNkMDBhMWQxZTQ3YzkxZDcxNjk5ZGQ5YzdlZjg2MWExMmYxZWZjMDhiMWFmMzczIn19fQ==
                Slots:
                - 22
                Title: "&b&lBuycraft&f&l:"
                Lore:
                - "&f- &7Klik for at åbne!"
                Settings:
                    ClickAction:
                    - '[PLAYSOUND] ORB_PICKUP'
                    - '[OPEN] CATEGORY'
            '5':
                Item: player head
                Value: eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvZTIwNjQwMzZiMjMyYmVkNGNkMDBhMWQxZTQ3YzkxZDcxNjk5ZGQ5YzdlZjg2MWExMmYxZWZjMDhiMWFmMzczIn19fQ==
                Slots:
                - 20
                Title: "&b&lInformation&f&l:"
                Lore:
                - "&f- &7Du har &b&n{PLAYER_COINS}&7 coins!"
                - ' '
                - "&7Brug denne kommando for at købe flere!:"
                - "&b/buy request <antal>"
                - ' '
                - "&7Købshistorik:"
                - '{PLAYER_PURCHASES}'
```



Der er også en Messages.yml, hvor du kan ændre teskten, prefix og andet:

```
Messages:
    prefix:
        success: "&8&l[&a&l!&8&l]&f"
        error: "&8&l[&c&l!&8&l]&f"
        warning: "&8&l[&3&l!&8&l]&f"
    currency:
        singular: coin
        plural: coins
    Buycraft_Info:
        CommandMessage:
        - " &8[ &b&lBUYCRAFT &8]"
        - ''
        - "&f/buycraft info\n   &f - &7Viser denne besked!"
        - "&f/buycraft info <player>\n   &f - &7Viser spillerens information!"
        - "&f/buycraft give <player> <amount>\n   &f - &7Giver Coins til spilleren! &nBliver logged som i købshistorik!"
        - "&f/buycraft take <player> <amount>\n   &f - &7Fjerner Coins fra spilleren! &nFjerner ikke fra købshistorik!"
        - "&f/buycraft clear <player>\n   &f - &7Resætter spillerens Coins og købshistorik!"
        - ''
        PlayerStats:
        - " &8[ &b&lBUYCRAFT &8]"
        - "&fSpiller: {PLAYER_NAME}"
        - "&fCoins: {PLAYER_COINS}"
        - 'Købshistorik:'
        - '{PLAYER_PURCHASES}'
        - "&f/buycraft take <player> <amount>\n   &f - &7Fjerner Coins fra spilleren! &nFjerner ikke fra købshistorik!"
        - "&f/buycraft clear <player>\n   &f - &7Resætter spillerens Coins og købshistorik!"
        - ''
```
