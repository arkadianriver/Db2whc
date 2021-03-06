---

copyright:
  years: 2014, 2018
lastupdated: "2018-09-25"

---

<!-- Attribute definitions --> 
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:pre: .pre}

# Installazione del pacchetto del driver su Mac OS X

Puoi installare il pacchetto del driver {{site.data.keyword.dashdbshort_notm}}su Mac OS X utilizzando lo script `installDSDriver.sh`.
{: shortdesc}

## Prerequisiti

Prima di tentare di collegarti al tuo database {{site.data.keyword.dashdbshort_notm}}, verifica di avere i [prerequisiti](connecting.html#prereqs) necessari.

<!-- Download the Db2 driver package for your operating system from the web console and install it. -->

## Procedura

- **Per una nuova installazione**

  1. Monta l'immagine del disco facendo doppio clic sul file `macos_dsdriver.dmg`. 
   
     Viene visualizzata una nuova finestra **Finder** con il contenuto dell'immagine del disco.

     Se la finestra **Finder** non si apre, fai doppio clic sull'icona `macos_dsdriver` sul tuo desktop.
  2. Nella finestra **Finder**, fai doppio clic sul file `installDSDriver.sh`.

     Il package del driver viene installato nell'ubicazione predefinita: `/Applications/dsdriver`.

- **Per aggiornamenti alla tua installazione del pacchetto del driver esistente**

  1. Esegui il backup dei file di configurazione correnti:

     a. Vai alla cartella `Applications/dsdriver/cfg`.

     b. Copia i seguenti file in una cartella diversa: 
    
        `db2cli.ini`

        `db2dsdriver.cfg`
  2. Rimuovi il pacchetto del driver attualmente installato facendo clic con il tasto destro del mouse sulla cartella `dsdriver` e selezionando **Move to Trash**.
  3. Installa il nuovo pacchetto del driver come descritto nella precedente sezione **Per una nuova installazione**:
     
     a. Monta l'immagine del disco facendo doppio clic sul file `macos_dsdriver.dmg`. 
     b. Nella finestra **Finder**, fai doppio clic sul file `installDSDriver.sh`.
  4. Ripristina i file di configurazione:

     Copia i file `db2cli.ini` e `db2dsdriver.cfg` che hai salvato dal passo 1 nella cartella `/Applications/dsdriver/cfg`.

## Operazioni successive

Per poter collegare le tue applicazioni locali o i tuoi strumenti client al tuo database {{site.data.keyword.dashdbshort_notm}}, [configura il tuo ambiente locale](driver_pkg_cfg.html).
