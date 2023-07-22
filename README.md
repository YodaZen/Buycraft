# Buycraft til Superawesome servere!

Dette er et specielt desginet Buycraft, lavet med henblik på at gøre det bruger venligt!

For at kunne benytte dette skal du have følgende plugins:

**Skript 2.6.4 (Anvend venligst en fork til 1.8)**

**Skript-Yaml 1.4.1**

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

Konfigurationsfilen, config.yml, kan findes ved følgende sti: _plugins/Skript/YAML/Buycraft/config.yml_

Vi håber, at vores Buycraft tilbyder dig en enestående mulighed for at udvide og tilpasse dit serverens købeprocess på bedst mulig vis.
```
Buycraft:
    Ranks:
        Item: player head
        Value: eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvZDMwZjcxMDE1NzZmMDQxNmJjZjQ4Yjc2Y2MwMGY2NzI0MmE5OTU2MGI4Yjg5M2MyMGIyMGRjODVjYTYzYjUyNyJ9fX0=
        Slot: 12
        Title: "&b&lRANKS&f&l:"
        Lore:
        - ' '
        - "&7Klik for at åbne!"
        Rank1:
            Priority: 1
            Item: player head
            Value: eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvYTc0ZjkxMGNhN2VkNzNkOGM1ZmRjODQ3NmQxYmVkN2FlNGUxOGY4ZTFkZjZiODAwZDE2YjNiZTNkMzNlYmJmYyJ9fX0=
            Price: 2500
            Slot: 12
            Title: "&b&lRANK &f&l1"
            Lore:
            - "&8|&m------------------&8|"
            - "&b&lRANK1 &f{PLAYER_NAME}"
            - "&fIndhold:\n&f - &7/Kit Ice (12h cooldown)"
            - "&f - &7/eat (5m cooldown)"
            - ' '
            - "&fPris: &b&n2.500 shards"
            - ' '
            - "&8|&m------------------&8|"
        Rank2:
            Priority: 2
            Item: player head
            Value: eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvYTM1NWMyZmNlNjIyNjM4YTQ2ZWM3ZTk2YTA5N2FjZWIzYjEyM2MwOTU4Y2MxMzExMjY4YWFkYzU2NTkyNDQzOSJ9fX0=
            Price: 5000
            Slot: 13
            Title: "&b&lRANK &f&l2"
            Lore:
            - "&8|&m------------------&8|"
            - "&b&lRANK2 &f{PLAYER_NAME}"
            - "&fIndhold:\n&f - &7/Kit Ice (12h cooldown)"
            - "&f - &7/eat (5m cooldown)"
            - ' '
            - "&fPris: &b&n5.000 shards"
            - ' '
            - "&8|&m------------------&8|"
        Rank3:
            Priority: 3
            Item: player head
            Value: eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvNGUyMWQyY2E5MjI3ZmRjMjIwYjMyYTk5OTA4NDNhMzRjN2U5NzVlZWM1OTVkMGYxMzdlMjUwYzE0Y2Q5NzI0NiJ9fX0=
            Price: 10000
            Slot: 14
            Title: "&b&lRANK &f&l3"
            Lore:
            - "&8|&m------------------&8|"
            - "&b&lRANK3 &f{PLAYER_NAME}"
            - "&fIndhold:\n&f - &7/Kit Ice (12h cooldown)"
            - "&f - &7/eat (5m cooldown)"
            - ' '
            - "&fPris: &b&n10.000 shards"
            - ' '
            - "&8|&m------------------&8|"
```
