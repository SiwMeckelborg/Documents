---
title: Installasjonsguide for einnsyn-klienten
description: Dokumentasjon for einnsyn-klient
summary: "Dokumentasjon for einnsyn-klient"
permalink: einnsyn_index.html
sidebar: einnsyn_sidebar

---

## [Nyeste versjon av einnsyn-klienten finner du her](https://github.com/difi/einnsyn-klient/releases/)

## Hvordan fungerer einnsyn-klienten

I de fleste tilfeller vil det være naturlig å sette opp både integrasjonspunktet og einnsyn-klient på samme server. Denne veiledningen tar utgangspunkt i det. 

Integrasjonspunktet er kanalen til omverdenen og må ha portåpning igjennom branmmuren. Samtidig må både einnsyn-klient og integrasjonspunkt ligge innenfor brannmur siden kommunikasjon går ukryptert til einnsyn-klient og arkivsystemet. Integrasjonspunktet må også ha tilgang til arkivsystemet for å kunne fungere for alternativ 1, og i tilfeller der innholdsleverandør skal sende andre meldinger enn eInnsyn-meldinger. 

eInnsyn-klienten kommuniserer over HTTP med integrasjonspunktet og trenger dermed tilgang til det. Siden innsynskrav blir sendt på e-post fra eInnsyn-klient til arkivsystem eller anna e-postboks trenger også klienten tilgang til en SMTP-server. [Mer om dette her](https://difi.github.io/einnsyn-klient/innsynskrav.html)

Filkatalogen (inputDirectory) er grensesnittet for arkivar. eInnsyn-klienten må kunne overvåke og skrive til denne katalogen. Samtidig må arkivar ha tilgang denne for å kunne laste opp filer. Dette forbeholder at filene ligger på en server som både arkivar har tilgang til, og som kommunisere med de andre komponentene. 

[Installasjonsveiledning for integrasjonspunktet finner du her](http://difi.github.io/move-integrasjonspunkt/vStaging/)

