---
name: addestra-comportamento-chatbot
description: "Reconstructs the intention a chatbot missed in its last saved conversation and repairs the cause in the prompt, tools or code. Use when a project's chatbot answered badly, made things up or ignored a request."
---

# Ripara comportamenti del chatbot

Appena ricevi questo prompt, come prima azione trova dove questo progetto persiste le conversazioni del chatbot, leggi l'ultima e parti da quel transcript. Non chiedere conferma, non iniziare dal codice di riparazione, non inventare il dialogo: se non la recuperi, fermati e chiedi solo dove trovarla.

Gli errori raramente sono evidenti a una lettura passiva. Non cercare bug in superficie: entra nel merito di ciò che il richiedente voleva e di come il chatbot ha disatteso quell'intenzione, anche quando la risposta sembra plausibile. Ricostruisci turno per turno obiettivo, vincoli e risultato atteso, cosa ha fatto il bot, e in quali modi concreti l'intenzione è stata disattesa, anche solo in parte. Distingui fallimenti palesi da fallimenti sottili: misconception rafforziate o non smontate, risposte alla lettera ma non allo scopo, omissioni che cambiano l'utilità del risultato. Non correggere ancora nulla.

Traduci ogni disallineamento in segnali da indagare a fondo nel codice, nei prompt e nei tool — non saltare al patch. Forma utile: «l'utente chiedeva X; il bot ha fatto Y → verificare Z nel routing / tool / system prompt»; «ha trattato A come B → dove nasce questa misconception nel flusso?»; «ha omesso C decisivo → quale passo obbligatorio manca o è opzionale per sbaglio?». Elenca solo ciò che emerge dal transcript, con riferimento al turno: errori fattuali, logici o di dominio; comportamenti vietati dalle regole del prodotto; omissioni critiche; improvvisazione al posto di policy, prompt o codice; misconception non corrette.

Per ogni segnale individua la causa a monte, non il sintomo, cercando nell'ordine più utile: istruzioni di sistema e policy; tool, retrieval o dati; codice di orchestrazione, guardrail e routing; ambiguità dell'input utente solo se è davvero dominante. Distingui causa da effetto: «ha inventato un prezzo» è l'effetto; la causa può essere l'assenza di un tool obbligatorio o una regola che non vieta le stime.

Ripara alla radice riscrivendo, non impilando. Preferisci riscrivere il pezzo di flusso, prompt o codice che produce l'errore, così il comportamento corretto diventa il percorso naturale e lo stesso fallo o misconception simili non si ripresentano. Non aggiungere wrapper, guardrail extra, liste di eccezioni o patch «se vedi questo caso allora…» che mascherano il problema lasciando intatta la logica sbagliata. Una regola chiara e strutturale, un vincolo obbligatorio nel codice o nel tool, e un test di regressione se il progetto lo prevede, bastano più di un elenco di casi speciali. Non correggere ad hoc solo il messaggio sbagliato della chat; dove tocchi il punto rotto, riscrivilo in modo che la classe di errori non possa ripetersi, senza allargare a refactor inutili.

Alla fine spiega in breve quale intenzione è stata disattesa, qual era la causa profonda, cosa hai riscritto e dove, e perché una conversazione equivalente non dovrebbe più produrre lo stesso errore o misconception simili. Segnala eventuali rischi residui in una riga.

Non leggere la conversazione in modo passivo. Non riparare impilando layer sopra una logica che resta sbagliata. Non riscrivere l'intera personalità del chatbot per un singolo incidente, non aggiungere liste lunghe di divieti, e non dichiarare risolto un problema se hai solo patchato la risposta superficiale.
