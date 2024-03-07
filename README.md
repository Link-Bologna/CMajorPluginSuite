# CMajorPluginSuite

## Cosa realizzeremo
L’idea di questo laboratorio collaborativo é di sviluppare una suite completa di plug-ins audio scritte in [Cmajor](https://cmajor.dev) per essere utilizzate in qualsiasi Digital Audio Workstation caricandole attraverso la precompilata [CMajor VST/AU plugin](https://github.com/cmajor-lang/cmajor/releases) che funziona su Linux, macOs e Windows.
Abbiamo pensato che per rendere ancora piú facile tanto il design quanto il test e lo sviluppo delle plug-ins, utilizzeremo in una prima frase l'[editor online](https://faustide.grame.fr/) [Faust](https://faust.grame.fr/) che permette di esportare il codice scritto in Faust in un progetto CMajor.
Approfondiremo i fondamenti di Faust e CMajor e le tecniche di base di elaborazione numerica di segnali (o [Digital Signal Processing](https://en.wikipedia.org/wiki/Digital_signal_processing) necessarie per la progettazione di sintetizzatori ed effetti audio.

## Getting started
- Naviga sul URL del nostro [editor online](https://faustide.grame.fr/)    
  - Questo sarà il tuo spazio di sviluppo
- Apri e leggi la documentazione di [Faust](https://faustdoc.grame.fr/) e delle [Faust Libraries](https://faustlibraries.grame.fr/)
- Sbizzarisciti e crea quello che ti serve ;)
- Scarica la versione precompilata [CMajor VST/AU plugin](https://github.com/cmajor-lang/cmajor/releases) 
  - Consigliamo una versione stable  
- Inserisci il nostro "contenitore plug-in" al interno della tua DAW preferita
  - trovi maggiori informazioni sulla documentazione di [specifica](https://cmajor.dev/docs/GettingStarted#loading-patches-in-your-daw-with-the-cmajor-vstau-plugin)
- Prova ad aprire il VST "vuoto" dovrebbe chiederti di inserire una patch
  - bene! siamo arrivati al punto saliente
- Esporta il file creato al interno del IDE con impostazioni "Platform" e "Architecture": Cmajor 
  - C'è un apposito button nella sezione di sinistra del editor online
  - Ci siamo quasi, tieni duro :)
- Verranno generati due file: 
  - uno sarà con estensione .cmajor e conterrà il codice sorgente vero e proprio della tua patch
  - uno con estensione .cmajorpatch e invece sarà il puntatore e los trumento di controllo del nostro codice sorgente
-  La patch (.cmajorpatch) generata dal nostro IDE e scaricata, ora puo essere spostata attraverso drag n drop direttamente dentro il nostro plugin 