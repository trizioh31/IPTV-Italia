# IPTV-Italia

Lista personale di canali TV italiani in formato M3U, aggiornata automaticamente.

## File nella repository

| File | Cosa è |
|------|--------|
| `iptvitaplus.m3u` | la lista attiva — è questa che va aperta in TiviMate, VLC, Kodi o simili |
| `iptvitaplus_oldcategory.m3u` | la versione precedente, con i canali raggruppati per categoria: la tengo come riferimento |
| `logos/` | immagini dei canali |

## Come nasce questa lista

Questa repository nasce come **fork di [Tundrak/IPTV-Italia](https://github.com/Tundrak/IPTV-Italia)** e per
anni il contenuto è stato quello del fork. Da novembre 2026 non è più così: la lista è generata dalla
pipeline di **[Ric-82/iptv-italia-builder](https://github.com/Ric-82/iptv-italia-builder)**.

La pipeline raccoglie i canali da liste pubbliche, li unifica per nome, sceglie per ogni canale il flusso
migliore preferendo i domini ufficiali degli editori (`rai.it`, `mediaset.net`, `la7.it`…) ai re-streamer,
e verifica che i flussi rispondano prima di pubblicarli.

Il fork di Tundrak resta il parente da cui è partito tutto: non è più la fonte dei canali.

## Aggiornamenti

Gli aggiornamenti sono automatici: i commit portano il messaggio `aggiornamento automatico`.

Il tag **`prima-di-ric82`** segna l'ultima lista precedente al cambio di sistema: per tornare indietro
basta fare il checkout di quel tag.

## EPG

L'header del file dichiara la guida programmi:

```
x-tvg-url="https://iptv-epg.org/files/epg-it.xml"
```

## Note

I flussi sono quelli pubblicati dagli editori e sono pensati per la visione all'interno dell'Italia.
Questa repository non ospita contenuti: contiene soltanto indirizzi.