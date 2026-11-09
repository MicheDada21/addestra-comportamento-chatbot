# ripara-comportamenti-chatbot

Indaga l'intenzione disattesa in una chat, traduce i fallimenti in segnali da verificare nel codice e riscrive alla radice perché non si ripetano.

Fa parte della [Prompt Library di CH Labs](https://www.cryptohelvetia.com/ch-labs/prompt-library), dove la pagina di riferimento è [Ripara comportamenti del chatbot](https://www.cryptohelvetia.com/ch-labs/prompt-library/skills/ripara-comportamenti-chatbot). Il repo contiene una copia della skill, rigenerata a ogni aggiornamento della libreria.

## Installare

In Claude Code aggiungi una volta il marketplace e installa il plugin.

```
/plugin marketplace add MicheDada21/ch-labs-skills
/plugin install ripara-comportamenti-chatbot@ch-labs-skills
```

Da shell i comandi sono `claude plugin marketplace add MicheDada21/ch-labs-skills` e `claude plugin install ripara-comportamenti-chatbot@ch-labs-skills`. Nell'app desktop premi + accanto al campo del prompt, apri Plugins, aggiungi il marketplace `MicheDada21/ch-labs-skills` con Add marketplace e poi il plugin con Add plugin.

Per avere tutte le skill della libreria installa `tutte-le-skill@ch-labs-skills`. Con altri agenti copia la cartella `skills/ripara-comportamenti-chatbot` tra le skill dell'agente, per esempio in `~/.codex/skills/ripara-comportamenti-chatbot`.

## Licenza

MIT, testo completo in [LICENSE](LICENSE).
