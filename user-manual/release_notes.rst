================
Note di rilascio
================

Cambiamenti principali - v3.4.0 - (12 NOV 2018)
===============================================

**Nuove funzionalità**

- `Possibilità di effettuare chiamate in maniera non autenticata: <https://nethvoice.docs.nethesis.it/it/v14/howto.html#product-cti-effettuare-chiamate-in-maniera-non-autenticata>`_ un esempio di utilizzo è l'esecuzione di chiamate in software di terze parti senza sviluppare necessariamente la parte di autenticazione. Leggendo attentamente la documentazione relativa, si nota che la funzione è **disabilitata di default** e può essere selettivamente attivata per **specifici range di indirizzi IP.**

**Bug fixes**

- Risolto il problema della scomparsa del pulsante "Cambia dispositivo": durante una chiamata è possibile "passare" la conversazione su un altro dispositivo associato al proprio utente

  - https://github.com/nethesis/dev/issues/5510
  - https://github.com/nethesis/dev/issues/5511

.. image:: img/switch-device.png



Cambiamenti principali - v3.3.3 - (5 NOV 2018)
===============================================

**Bug fixes**

- `Sistemato il "freeze" del client quando si eseguiva il reload del server in presenza di centinaia di utenti configurati <https://github.com/nethesis/dev/issues/5504>`_
- `La rest api "astproxy/extension" restituiva il risultato anche in assenza dell'header HTTP Authorization <https://github.com/nethesis/dev/issues/5501>`_
- `Rimossa la doppia richiesta del client per ottenere la lista delle chiamate perse in coda: avveniva dopo un reload del server <https://github.com/nethesis/dev/issues/5500>`_
- `Dopo un reload del server e in caso di "DND on/off automatico" dell'utente scelto dal client, il log del server riportava degli errori a causa dell'esecuzione di operazioni duplicate <https://github.com/nethesis/dev/issues/5495>`_

.. _SO: http://stackoverflow.com/

Cambiamenti principali - v3.3.2 - (31 OTT 2018)
===============================================

**Bug fixes**

- `Sistemata la registrazione dei messaggi audio nel servizio "Fuori Orario" <https://github.com/nethesis/dev/issues/5492>`_
- `Rubrica: <https://github.com/nethesis/dev/issues/5485>`_

  - rimosso il pulsante "modifica" sui contatti provenienti dalla rubrica centralizzata
  - sistemata la ricerca alfabetica quando si utilizza la visualizzazione per "azienda"
  - rimosso il pulsante "speeddial" durante la modifica di un contatto non proprio
- `Il click sul popup di arrivo chiamata non portava in primo piano il tab NethCTI <https://github.com/nethesis/dev/issues/5484>`_
- `Le pagine dei servizi senza permesso erano raggiungibili anche se vuote <https://github.com/nethesis/dev/issues/5484>`_

Nuova versione |version|
========================

|product| versione |version| introduce una nuova grafica, completamente rinnovata e semplificata per l'utente finale.

Funzionalità principali:

- Configurazione semplificata attraverso il wizard di |parent_product|
- Salvataggio centralizzato sul server di tutte le preferenze utente
- Customer card più semplici da configurare e con una veste grafica completamente rivista
- Gestione device multipli associati ad un singolo utente
- Possibilità di impostare la presence in modo unificato su tutti i dispositivi
- Personalizzazione avatar
- Nuova chat (XMPP)
- Restyling grafico e funzionale del pannello operatore
- Possibilità di raggruppare i risultati della ricerca in rubrica per persona o per azienda
- Nuovo softphone WebRTC con supporto alle videochiamate (solo fra interni WebRTC)
- Visualizzazione sorgenti video anche dall'esterno della LAN
- Conferenze audio
- Configurazione servizio notte
- Code: chiamate perse, login e logout automatico
- Visualizzazione stato dei fasci
- Apertura di un url parametrizzato in corrispondenza della ricezione di una chiamata
- Nethifier
- Supervisore Code

Le seguenti funzioni non sono disponibili:

- Post-it e note chiamate
- Sedi remote
- Integrazione SMS e notifiche offline (mail e SMS)
- Inoltro della chiamata a numero o voicemail, su non disponibile/occupato
- Script personalizzati per la gestione chiamate
- Posto Operatore

.. warning:: |product| |version| necessita di |parent_product| 14