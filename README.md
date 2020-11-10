# homeassistant-package-consumi

package consumi
<img src="https://github.com/robertopiumatti/hassio-package-consumi/blob/main/consumi-gif.gif">

**Contributi:**
- il progetto parte lavoro di Mauro Cimino (https://hassiohelp.eu/2019/03/02/controllo-consumi-costi/, https://hassiohelp.eu/author/legolas08/)
- poi modificato da Domenico Ceccarelli (https://github.com/riddik14/hassio-package-consumi)

**Implementazioni**
- Implementazione gestione dei tre tipi di tariffazione (monoraria F1, bioraria F1-F23, trioraria F1-F2-F3)
- calcolo della stima bolletta italiana con la maggior precisione possibile: inseriti i calcoli precisi trasporto, oneri di sistema e accise presi dal sito isitituzionale ARERA

**INSTALLAZIONE**
1. copiare il file *pkg_tariffe_luce_consumi.yaml* nella cartella '/config/packages'
2. modifare il file *pkg_tariffe_luce_consumi.yaml*  alla riga 21 per inserire il sensore di energia
(Solo nel caso non si abbia un sensore di energia, ma solo quello di potenza instantanea seguire le istruzioni dalla riga 23 in poi)

**CREAZIONE LOVELANCE CARD**
1. installare dal menu frontend di hacs i seguenti:
	- vertical-stack-in-card
	- mini-graph-card
	- banner-card
	- paper-buttons-row
	- state-switch
2. creare card manuale su lovelance e copiare il contenuto del file lovelace-dash.yaml

**SETTING**
Trovate sia nel package che al fondo della card tutti i parametri da configurare.

**Materia Energia**
Potete trovare le tariffe (F1,F2,F3) sulla bolletta. 
Invece la quota fissa della materia energia dovrebbe essere sul contratto con il vostro fornitore (di norma intorno ai 50€) o sulla bolletta.
 - Materia Energia Quota Fissa Annua 
 - TariffaF1
 - TariffaF2
 - TariffaF3

**Trasporto costi unitari**
- KwContatore: inserire i KW del proprio contatore (di norma 3kW)
- TrasportoQuotaFissaAnnua: 20.4000€ (valore preso dal sito ARERA)
- TrasportoQuotaPotenzaAnnua: 20.8800€ (valore preso dal sito ARERA)
- TrasportoQuotaEnergia: 0.00833000€ (valore preso dal sito ARERA)

**Oneri Di Sistema costi unitari **
- OneriDiSistemaQuotaEnergia:  0.041817€ (valore preso dal sito ARERA)

**Accisa costi unitari  **
- Accise: 0.0227€ (valore preso dal sito ARERA)

** IVA**
- Iva: 10%






