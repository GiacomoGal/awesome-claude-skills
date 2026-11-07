# Guida di ingresso — fork GiacomoGal/awesome-claude-skills

Questa guida è l’ingresso documentale del fork. Descrive il tree osservato, i contratti già scritti e i vincoli di questa lettura. È pronta per una review indipendente. Non assegna un PASS, non dichiara il repository funzionante e non attesta un uso corrente.

La guida agente coerente è [AGENTS.md](AGENTS.md). Gli identificatori `F*`, `U*`, `N1` e `M*` sono gli stessi nei due file.

## Stato osservato

Controllo eseguito sul checkout Cloud Agent il 2026-11-07, in sola lettura sui metadati pubblici e sul file presente. Il ref di inventario `main` coincide con il default branch e con `origin/main`. Questa coincidenza di nome e di puntatore git non è una prova di allineamento a una VPS.

| Fatto | Valore osservato |
|---|---|
| URL del fork | https://github.com/GiacomoGal/awesome-claude-skills |
| Default branch | `main` |
| Base di questa guida | `2bbfe8b9779aeb34c619446efd7ea0a139a90658` |
| Oggetto del commit | Merge pull request #11 from zacharyr0th/add-claude-starter |
| Autore git del commit | Behi |
| Data del commit | 2025-11-23 13:15:51 +0330 |
| Tree a quel commit | solo `README.md` |
| Fork | sì |
| Archivio | no |
| Licenza dichiarata da GitHub | nessuna |
| Linguaggio primario dichiarato da GitHub | nessuno |
| Descrizione GitHub | A curated list of Claude Skills. |
| Parent | https://github.com/BehiSecc/awesome-claude-skills |
| Punta upstream `main` | `adf99015a0ad4dac11711c261f0f9b433e4215e7` |
| Confronto GitHub base…upstream | status `ahead`, `ahead_by` 246, `behind_by` 0, `total_commits` 246 |
| URL del confronto | https://github.com/BehiSecc/awesome-claude-skills/compare/2bbfe8b9779aeb34c619446efd7ea0a139a90658...adf99015a0ad4dac11711c261f0f9b433e4215e7 |
| Tree upstream alla punta | `README.md`, `atlas.svg`, `apimart.jpeg` |

`behind_by` 0 indica che la base del fork è antenata della punta upstream: alla data del controllo il fork non aveva commit propri sopra quell’antenato. I 246 commit upstream non sono stati letti uno a uno e non sono stati recuperati nel clone. Questa PR non li unisce.

Dal mandato di sezione 6, riportato come dato di mandato e non come misura nuova: `identity_proven` falso, uso corrente sconosciuto, perimetro documentale `unresolved`, `identity_evidence` vuota, proposte ed esecuzioni vuote. UNMAPPED: nessuna associazione, nel mandato, fra questo nome e un repository omonimo o un servizio VPS; identità d’uso e installazione non accertate. Nel tree locale non c’è un documento di installazione o di uso. La metà VPS del dato UNMAPPED resta un dato di mandato: questo ingresso non ha interrogato host, inventari esterni o servizi.

## Cosa contiene il tree

`README.md` è un elenco curato di link a skill Claude, più una procedura di contributo e un contatto. Non contiene corpi di skill, `SKILL.md`, script, lockfile, configurazione, licenza, né una guida di installazione del catalogo stesso.

L’avviso in cima al README di questa PR è l’unico adattamento del testo di catalogo. Sposta di due righe il contenuto che al commit base inizia alla riga 3. Le righe citate sotto come fonte sono quelle di `2bbfe8b9779aeb34c619446efd7ea0a139a90658`. Nel README di questa PR la riga nuova è la riga base più 2, per ogni riga base maggiore o uguale a 3.

## Matrice delle fonti verso il testo nuovo

| ID | Fonte | Riga | Contenuto usato | Destinazione | Motivo |
|---|---|---|---|---|---|
| S1 | Mandato, vincoli comuni | 5 | Guide Markdown di ingresso, specifiche del repository; lettura delle istruzioni esistenti e annidate prima di scrivere; matrice con fonte, riga, rango, destinatario, condizioni e destinazione | Questa guida e `AGENTS.md` | Il tree ha un solo file. La guida descrive quel file e il rapporto col parent, senza un modello riusabile su altri repository |
| S2 | Mandato, vincoli comuni | 5 | Conservare guardrail, permessi e letture host anche quando assenti; tenere cataloghi, commenti, prompt e manuali nel loro rango | Righe `F2`–`F9`, `F8`, `N1`, `M5` | Il README non contiene un permesso di lettura host. L’assenza resta scritta, così non diventa un permesso implicito |
| S3 | Mandato, vincoli comuni | 5 | Dichiarare i conflitti e lasciarli aperti sul piano operativo | Sezione «Conflitti aperti» | La divergenza col parent e i trigger del catalogo restano dichiarati |
| S4 | Mandato, vincoli comuni | 6 | Nessuna modifica a codice, config, script, dati, media, lock; verifiche documentali e link statici; effetti e limiti espliciti; niente auto-PASS | Diff limitato a Markdown; sezione link; ricevuta | Il controllo link registra lo stato HTTP e il suo limite |
| S5 | Mandato, vincoli comuni | 6–7 | PR Markdown sul fork, SHA base e head, niente force push né rebase condiviso, review indipendente prima di un PASS solo documentale | Ricevuta e descrizione della PR | La consegna è il testo, non un’integrazione |
| S6 | Mandato, vincoli comuni | 7 | Nel fork si conserva l’upstream; gli adattamenti sono quelli necessari; nessuna PR upstream | Avviso nel README; righe `U*` | L’avviso nomina il parent e non riscrive contributo, contatto o voci |
| S7 | Mandato, sezione 6 | 81–94 | URL, `main`, fork, non archiviato, UNMAPPED, guida esplorativa, output con SHA e limiti | Sezione «Stato osservato» | I metadati git e GitHub confermano ref, fork e tree; l’uso resta sconosciuto |
| S8 | `README.md` del fork al base | 1–108 | Contratti e catalogo già nel file | Matrice obblighi `F*` | Fonte diretta del testo che un lettore trova nel checkout |
| S9 | `README.md` upstream `adf99015` | 3–6, 28–29, 337–349 | Sponsor, consiglio, contributo e contatto alla punta upstream | Matrice `U*` | Confronto di contratto. Il file upstream non è stato copiato nel fork |

## Matrice degli obblighi, dal testo precedente al testo nuovo

Rango, destinatario e condizione valgono per la destinazione indicata. Una riga di rango `catalogo` o `trigger-di-catalogo` resta una citazione del README.

| ID | Fonte | Riga | Rango | Destinatario | Condizione | Obbligo precedente | Destinazione |
|---|---|---|---|---|---|---|---|
| F1 | README fork @ `2bbfe8b` | 1 | identità del file | Chi apre il README | All’apertura del file | Il documento si intitola «Awesome Claude Skills» | Titolo invariato. L’avviso di fork sta sotto il titolo e non lo sostituisce |
| F2 | README fork @ `2bbfe8b` | 4–94 | catalogo | Chi consulta l’elenco | Quando legge una voce per orientarsi | Elenco di link con descrizioni di terzi, in dieci sezioni dal Document Skills allo Utility & Automation. Le descrizioni comprendono azioni nominate, fra cui git automatizzato (riga 75), fuzzing FFUF (riga 83), test di web app con Playwright (riga 85), organizzazione di file (riga 91) e organizzazione di fatture (riga 92) | Testo delle voci invariato. Rango conservato come catalogo. Le azioni nominate restano descrizioni di risorse esterne. Questa guida non le trasforma in passi eseguibili |
| F3 | README fork @ `2bbfe8b` | 27 | trigger di catalogo | Lettore della voce `test-driven-development` | Quando legge quella voce | Citazione: «Use when implementing any feature or bugfix, before writing implementation code» | Citazione conservata nel README. Nella sessione di questo ingresso il trigger resta nel rango catalogo e il contenuto collegato resta non eseguito |
| F4 | README fork @ `2bbfe8b` | 39 | trigger di catalogo | Lettore della voce `root-cause-tracing` | Quando legge quella voce | Citazione: «Use when errors occur deep in execution and you need to trace back to find the original trigger» | Stessa destinazione di F3. Lo stato HTTP di questa URL, al controllo, è 404 |
| F5 | README fork @ `2bbfe8b` | 86 | trigger di catalogo | Lettore della voce `systematic-debugging` | Quando legge quella voce | Citazione: «Use when encountering any bug, test failure, or unexpected behavior, before proposing fixes» | Stessa destinazione di F3 |
| F6 | README fork @ `2bbfe8b` | 96–104 | procedura di contributo | Chi ha suggerimenti, miglioramenti o nuove risorse; in alternativa chi segnala un difetto | Se vuole proporre una modifica alla lista, oppure se nota qualcosa da correggere | «Fork this repo», «Make your changes», «Submit a Pull Request». In alternativa: aprire una Issue | Testo invariato (nel README di questa PR: righe 98–106). Ambiguità lasciata aperta: «this repo», letto sul fork, può indicare il fork o il parent. Questa PR non esegue la procedura verso il parent |
| F7 | README fork @ `2bbfe8b` | 106–108 | contatto | Chi vuole contattare l’autore indicato dal README («me») | Se vuole scrivere a quell’autore | «If you want to contact me, you can reach me on X», URL `https://x.com/Behi_Sec` | Testo invariato (nel README di questa PR: righe 108–110). Il contatto non è riscritto con l’owner del fork |
| F8 | README fork @ `2bbfe8b`; tree del commit; metadato licenza | intero file; tree | assenza | Agente e lettore del checkout | Quando si cerca un permesso, una licenza o un corpo di skill in questo repository | Nel file non c’è una concessione di lettura dell’host, un permesso su credenziali, una licenza, né un corpo di skill | L’assenza è registrata qui e in `AGENTS.md`. Non è convertita in permesso. I permessi eventuali vivono, se esistono, nei repository collegati e restano non letti (`N1`) |
| F9 | README fork @ `2bbfe8b` | 32 | trigger di catalogo | Lettore della voce `claude-starter` | Quando legge la pretesa di attivazione automatica | La voce attribuisce al progetto esterno «40 auto-activating skills» | Citazione invariata. L’attivazione automatica non è un trigger di questa sessione. Al controllo la URL risponde 404. Il numero e il meccanismo non sono verificati |
| U1 | README upstream @ `adf99015` | 28–29 | consiglio upstream | Chi usa Claude per costruire applicazioni web | Quando legge la punta upstream, non quando legge il fork | Alert `[!Tip]`: usare VibeSec-Skill «to avoid getting hacked», con link a `https://github.com/BehiSecc/VibeSec-Skill` | Registrato come consiglio della punta upstream. Assente nel README del fork. Non copiato nell’avviso, non adottato come policy di sessione, non installato |
| U2 | README upstream @ `adf99015` | 337–345 | procedura di contributo | Come F6 | Come F6 | Stesso testo di F6 | Il contratto di contributo alla punta upstream coincide con quello del fork. Nessuna delle due copie è stata modificata |
| U3 | README upstream @ `adf99015` | 347–349 | contatto | Come F7 | Come F7 | Stesso testo di F7 | Il contatto alla punta upstream coincide con quello del fork |
| U4 | README upstream @ `adf99015`; tree upstream | 3–6; file `atlas.svg` e `apimart.jpeg` | promozione upstream | Lettore della punta upstream | Quando apre la punta upstream | Tabella di sponsor con rimandi commerciali e due file media, assenti nel fork | Non importata. Il rango resta promozione della punta upstream, non norma del fork e non policy di sessione. I testi promozionali non sono ricopiati qui |
| U5 | API compare di GitHub sul parent | confronto citato sopra | metadato git | Chi valuta se allineare il fork | Quando confronta le due punte `main` | Il parent è 246 commit avanti; il fork è 0 commit avanti rispetto all’antenato comune che è la base stessa | Fatto registrato. Nessun merge, nessun fetch di quei commit, nessuna PR sul parent |
| N1 | URL nel catalogo del fork | 4–94, come link | contratto annidato non letto | Destinatari dei repository collegati, qui sconosciuti | Quando un lettore segue una URL fuori da questo tree | I corpi, i permessi, i trigger e le condizioni delle skill collegate non sono in questo repository | Restano non letti e non eseguiti. Il rango remoto non è accertato. Non leggerli non cancella un contratto che esista a destinazione e non crea un permesso locale |
| M1 | Mandato, sezione 6 e avvertenza di questo incarico | 81–94, più il vincolo che annulla audit e import | vincolo di ingresso | Autore di questa PR e agente sul checkout | Per tutto il lavoro di ingresso | L’incarico è l’ingresso documentale del repository. Audit del catalogo, import, installazione e modifica di skill globali sono fuori da questo incarico | Le guide e il diff Markdown. Le voci del catalogo non sono state corrette, aggiunte o rimosse |
| M2 | Mandato, sezione 6 | 86–91 | vincolo di ingresso | Lettore della guida | Finché una fonte ulteriore, fuori da questo ingresso, non accerta uso e installazione | Uso e installazione sono sconosciuti (UNMAPPED) | Sezioni stato e `AGENTS.md`. Nessuna procedura di installazione è stata inventata |
| M3 | Mandato, vincoli comuni | 6 | vincolo di ingresso | Agente sul checkout | Durante questa lettura e le successive che seguono queste guide | Segreti, env, config sensibili, backup, memorie, dati privati e host restano fuori dalla lettura | Nessun file di quel tipo è stato aperto. Le guide non indicano percorsi di quel tipo |
| M4 | Mandato, vincoli comuni | 6–7 | vincolo di ingresso | Chi pubblica la PR | Al push e verso il parent | Push ordinario. Il parent non riceve PR, merge, sync, deploy o archive da questo ingresso | Branch del fork e PR verso `main` del fork |
| M5 | Mandato di questo incarico | vincolo esplicito su cataloghi | vincolo di ingresso | Agente in sessione | Quando una voce, un esempio o un prompt del catalogo somiglia a un’istruzione | Cataloghi, esempi e prompt del README hanno il rango della loro riga `F*`, non il rango di policy di sessione | `AGENTS.md`, in apertura |
| M6 | Mandato, vincoli comuni e sezione 6 | 6 e 94 | vincolo di ingresso | Reviewer indipendente | Prima di qualunque PASS documentale | La PR è pronta per la review. Il PASS appartiene al reviewer | Ricevuta. Questa guida non contiene un PASS |

La riga F3 usa il verbo «adottato» nel senso di policy di sessione: il trigger resta visibile nel catalogo e non entra fra le istruzioni dell’agente.

## Conflitti aperti

Questi fatti convivono. Questo ingresso non ne chiude nessuno con una modifica operativa.

1. **Contributo.** F6 e U2 dicono di fare fork, modificare e aprire una Pull Request, oppure una Issue. M4 tiene questa PR sul fork `GiacomoGal/awesome-claude-skills` e lascia il parent intatto. Il testo di Contribution resta quello del base. La PR corrente non è l’esecuzione di F6 verso il parent. L’ambiguità di «this repo» resta aperta.
2. **Punta upstream.** U5 dice che il parent è 246 commit avanti e che la base del fork ne è antenata. U1 e U4 esistono solo sulla punta upstream. Il README del fork resta il testo del base, più l’avviso. I 246 commit, lo sponsor, i media e il consiglio VibeSec restano sul parent.
3. **Trigger.** F3, F4, F5 e F9 sono frasi imperative o di auto-attivazione dentro voci di catalogo. M5 assegna a quelle frasi il rango catalogo. Entrambe le cose sono vere insieme: la frase sta nel README; la sessione di ingresso non la esegue.
4. **Link e voci.** Diciassette URL del README rispondono HTTP 404 al controllo sotto. Le voci restano nel catalogo perché M1 esclude la revisione del catalogo. Lo stato HTTP e la presenza della voce sono due fatti paralleli.
5. **Contatto e owner.** F7 indica «me» e `https://x.com/Behi_Sec`. L’owner GitHub del fork è `GiacomoGal`. L’autore git del commit base si chiama Behi, come il login del parent `BehiSecc`. M2 tiene `identity_proven` falso. Lo stato HTTP 200 della pagina X non identifica chi usa oggi il fork.
6. **Contratti annidati.** N1 registra che i contratti nei repository collegati non sono stati letti. F8 registra che questo tree non contiene quei contratti. Le due assenze hanno destini diversi: il tree locale non concede permessi; il remoto può contenerne, e questo ingresso non li accerta.

## Controllo dei link

Controllo del 2026-11-07 sulle 44 URL assolute del README al commit base. Comando, per ciascuna URL: `curl -I -L --max-redirs 5 --max-time 20`, senza header di autorizzazione e senza salvare il corpo. Effetto: uno status HTTP finale e, se c’è stato un redirect, la URL finale. Limite: lo status non conferma la descrizione della voce, il testo di una skill, la sicurezza, la licenza o l’installabilità. Un 200 dopo redirect non conserva il path originale. Un 404 è lo stato di quella URL in quel momento, non una patch proposta. Il corpo di `invoice-organizer/SKILL.md` non è stato scaricato. Il 200 di `https://x.com/Behi_Sec` dice che la pagina ha risposto, non chi opera il fork.

Esito: 27 URL con status finale `200`, 17 con status finale `404`. Nessun altro status e nessun errore di trasporto in questo passaggio.

| Voce | HTTP | Redirect | URL richiesta | URL finale, se diversa |
|---|---|---|---|---|
| docx | 404 | 0 | https://github.com/anthropics/skills/tree/main/document-skills/docx | — |
| pdf | 404 | 0 | https://github.com/anthropics/skills/tree/main/document-skills/pdf | — |
| pptx | 404 | 0 | https://github.com/anthropics/skills/tree/main/document-skills/pptx | — |
| xlsx | 404 | 0 | https://github.com/anthropics/skills/tree/main/document-skills/xlsx | — |
| artifacts-builder | 404 | 0 | https://github.com/anthropics/skills/tree/main/artifacts-builder | — |
| test-driven-development | 200 | 0 | https://github.com/obra/superpowers/tree/main/skills/test-driven-development | — |
| using-git-worktrees | 200 | 1 | https://github.com/obra/superpowers/blob/main/skills/using-git-worktrees/ | https://github.com/obra/superpowers/tree/main/skills/using-git-worktrees |
| finishing-a-development-branch | 200 | 0 | https://github.com/obra/superpowers/tree/main/skills/finishing-a-development-branch | — |
| pypict-claude-skill | 200 | 0 | https://github.com/omkamal/pypict-claude-skill | — |
| aws-skills | 200 | 0 | https://github.com/zxkane/aws-skills | — |
| claude-starter | 404 | 0 | https://github.com/raintree-technology/claude-starter | — |
| move-code-quality-skill | 200 | 0 | https://github.com/1NickPappas/move-code-quality-skill | — |
| claude-code-terminal-title | 200 | 0 | https://github.com/bluzername/claude-code-terminal-title | — |
| root-cause-tracing | 404 | 0 | https://github.com/obra/superpowers/tree/main/skills/root-cause-tracing | — |
| csv-data-summarizer-claude-skill | 200 | 0 | https://github.com/coffeefuelbump/csv-data-summarizer-claude-skill | — |
| scientific-databases | 404 | 1 | https://github.com/K-Dense-AI/claude-scientific-skills/tree/main/scientific-databases | https://github.com/K-Dense-AI/scientific-agent-skills/tree/main/scientific-databases |
| scientific-integrations | 404 | 1 | https://github.com/K-Dense-AI/claude-scientific-skills/tree/main/scientific-integrations | https://github.com/K-Dense-AI/scientific-agent-skills/tree/main/scientific-integrations |
| scientific-packages | 404 | 1 | https://github.com/K-Dense-AI/claude-scientific-skills/tree/main/scientific-packages | https://github.com/K-Dense-AI/scientific-agent-skills/tree/main/scientific-packages |
| scientific-thinking | 404 | 1 | https://github.com/K-Dense-AI/claude-scientific-skills/tree/main/scientific-thinking | https://github.com/K-Dense-AI/scientific-agent-skills/tree/main/scientific-thinking |
| article-extractor | 200 | 1 | https://github.com/michalparkola/tapestry-skills-for-claude-code/tree/main/article-extractor | https://github.com/michalparkola/tapestry-skills/tree/main/article-extractor |
| content-research-writer | 200 | 0 | https://github.com/ComposioHQ/awesome-claude-skills/tree/master/content-research-writer | — |
| internal-comms | 404 | 0 | https://github.com/anthropics/skills/tree/main/internal-comms | — |
| brainstorming | 200 | 0 | https://github.com/obra/superpowers/tree/main/skills/brainstorming | — |
| family-history-research | 200 | 0 | https://github.com/emaynard/claude-family-history-research-skill | — |
| tapestry | 404 | 1 | https://github.com/michalparkola/tapestry-skills-for-claude-code/tree/main/tapestry | https://github.com/michalparkola/tapestry-skills/tree/main/tapestry |
| ship-learn-next | 200 | 1 | https://github.com/michalparkola/tapestry-skills-for-claude-code/tree/main/ship-learn-next | https://github.com/michalparkola/tapestry-skills/tree/main/ship-learn-next |
| youtube-transcript | 200 | 1 | https://github.com/michalparkola/tapestry-skills-for-claude-code/tree/main/youtube-transcript | https://github.com/michalparkola/tapestry-skills/tree/main/youtube-transcript |
| video-downloader | 200 | 0 | https://github.com/ComposioHQ/awesome-claude-skills/tree/master/video-downloader | — |
| image-enhancer | 200 | 0 | https://github.com/ComposioHQ/awesome-claude-skills/tree/master/image-enhancer | — |
| claude-epub-skill | 200 | 0 | https://github.com/smerchek/claude-epub-skill | — |
| git-pushing | 200 | 0 | https://github.com/mhattingpete/claude-skills-marketplace/tree/main/engineering-workflow-plugin/skills/git-pushing | — |
| review-implementing | 200 | 0 | https://github.com/mhattingpete/claude-skills-marketplace/tree/main/engineering-workflow-plugin/skills/review-implementing | — |
| test-fixing | 200 | 0 | https://github.com/mhattingpete/claude-skills-marketplace/tree/main/engineering-workflow-plugin/skills/test-fixing | — |
| meeting-insights-analyzer | 200 | 1 | https://github.com/ComposioHQ/awesome-claude-skills/blob/master/meeting-insights-analyzer/ | https://github.com/ComposioHQ/awesome-claude-skills/tree/master/meeting-insights-analyzer |
| linear-cli-skill | 200 | 0 | https://github.com/Valian/linear-cli-skill | — |
| ffuf_claude_skill | 200 | 0 | https://github.com/jthack/ffuf_claude_skill | — |
| defense-in-depth | 404 | 0 | https://github.com/obra/superpowers/blob/main/skills/defense-in-depth | — |
| webapp-testing | 404 | 0 | https://github.com/anthropics/skills/tree/main/webapp-testing | — |
| systematic-debugging | 200 | 1 | https://github.com/obra/superpowers/blob/main/skills/systematic-debugging | https://github.com/obra/superpowers/tree/main/skills/systematic-debugging |
| file-organizer | 200 | 0 | https://github.com/ComposioHQ/awesome-claude-skills/tree/master/file-organizer | — |
| invoice-organizer | 200 | 0 | https://github.com/ComposioHQ/awesome-claude-skills/blob/master/invoice-organizer/SKILL.md | — |
| skill-creator | 404 | 0 | https://github.com/anthropics/skills/tree/main/skill-creator | — |
| template-skill | 404 | 0 | https://github.com/anthropics/skills/tree/main/template-skill | — |
| X (contatto) | 200 | 0 | https://x.com/Behi_Sec | — |

Durante la lettura del README upstream, la voce `docx` alla riga 33 punta a `https://github.com/anthropics/skills/tree/main/skills/docx`, path diverso da quello del fork. È un esempio di deriva del catalogo fra base e punta. I due elenchi non sono stati riconciliati e le URL upstream diverse non sono state ricontrollate: farlo sarebbe una revisione del catalogo upstream, fuori da M1.

## Perimetro di questa guida

L’ingresso copre il README del fork, il confronto di contratto con la punta upstream e lo status HTTP delle URL del fork. Restano fuori, per M1–M4: installare o importare skill, eseguire i contenuti collegati, correggere le voci, leggere segreti o l’host, aprire una PR sul parent, fare merge, sync, deploy o archive, e trattare le descrizioni dipendenti da file esterni come verificate. Le voci su fatture, database scientifici, file system e test di applicazioni descrivono risorse assenti da questo tree: il loro contenuto resta non verificato.

## Ricevuta

| Campo | Valore |
|---|---|
| Base | `2bbfe8b9779aeb34c619446efd7ea0a139a90658` |
| Branch | `cursor/ingresso-documentale-awesome-claude-skills-60f0` |
| Head | Lo SHA del commit che introduce questa guida. Va letto da git dopo il commit e dalla PR. Questo file non lo anticipa, perché scriverlo prima del commit lo renderebbe falso |
| Parent | `BehiSecc/awesome-claude-skills` @ `adf99015a0ad4dac11711c261f0f9b433e4215e7` |
| File toccati | `README.md` (solo l’avviso), `GUIDA-INGRESSO.md`, `AGENTS.md` |
| Esito di questo documento | Materiale per review indipendente. Il PASS documentale non è assegnato |
