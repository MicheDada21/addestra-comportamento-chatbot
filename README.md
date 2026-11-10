# addestra-comportamento-chatbot

Indaga l'intenzione disattesa in una chat, traduce i fallimenti in segnali da verificare nel codice e riscrive alla radice perché non si ripetano.

Fa parte della [Prompt Library di CH Labs](https://www.cryptohelvetia.com/ch-labs/prompt-library), dove la pagina di riferimento è [Addestra comportamento chatbot](https://www.cryptohelvetia.com/ch-labs/prompt-library/skills/addestra-comportamento-chatbot). Il repo contiene una copia della skill, rigenerata a ogni aggiornamento della libreria.

## Installare

In Claude Code aggiungi una volta il marketplace e installa il plugin.

```
/plugin marketplace add MicheDada21/ch-labs-skills
/plugin install addestra-comportamento-chatbot@ch-labs-skills
```

Da shell i comandi sono `claude plugin marketplace add MicheDada21/ch-labs-skills` e `claude plugin install addestra-comportamento-chatbot@ch-labs-skills`. Nell'app desktop premi + accanto al campo del prompt, apri Plugins, aggiungi il marketplace `MicheDada21/ch-labs-skills` con Add marketplace e poi il plugin con Add plugin.

Con altri agenti copia la cartella `skills/addestra-comportamento-chatbot` tra le skill dell'agente, per esempio in `~/.codex/skills/addestra-comportamento-chatbot`.

## Licenza

MIT, testo completo in [LICENSE](LICENSE).
