

# session plan


# session 1 - kick-off meeting + chat-based AI support

- who I am and my background

- ? who-is-who?
  + ? AI experiences / usage so far?
  
- ? what are open (AI-related) questions? (ggf. Abgabeübung vor sitzung?!)

- course layout
  - workflow
  - intro to ai-based tests of self-study + code-word submission
  - expectations and what to expect

- ? (how) did your "knowledge search strategy" changed since AIs are available?

- AI in chat-mode for coding
  - discussion on previous experiences
    - ? what platforms used/registered? 
      - allrounder: chatgpt, claude, gemini, ms copilot, deepseek, ... )
      - recherche: perplexity (mit quellenangabe)
      - coding: gh copilot, 
      - integration: Meta AI, ms copilot in Windows, apple intelligence, ...
    - ? why these? other tested?
  - ? how do you approach a coding problem using a chat AI?

- ! chat AI task
  - [session-1.handson.md](session-1.handson.md)
  - possible AI platforms (distribute among students)
    - chatgpt.com
    - copilot.microsoft.com
    - huggingface.co/chat
    - https://duckduckgo.com/chat
    - https://talkai.info/de/chat/
      - verschiedene modelle wählbar  - 


# 2 - self-study material

- github (copilot) registration
- visual studio code installation 
  - enabling github copilot
- https://medium.com/data-science-at-microsoft/how-large-language-models-work-91c362f5b78f
  - google translate link + hint about "audio option"
  - codeword test
- https://medium.com/@sukhitashvili.soso/choosing-temperature-topk-and-topp-for-llm-text-generation-7b0972a9bb2a

# session 2 - "context and IDE-internal autocompletion"

- model != "service/platform"
  - idR 2-3 Modellebenen, unterscheiden sich in 
    - input/context größe
    - modellumfang (speicher+verknüpfungen, anzahl parameter, ...)
    - reasoning-loops und "unsichtbarem denken" etc.

- temperature and top_p in action
  - https://medium.com/@sukhitashvili.soso/choosing-temperature-topk-and-topp-for-llm-text-generation-7b0972a9bb2a
  - https://chat-ai.academiccloud.de/
    - login with university account
    - select model
    - "settings" upper right corner
      - ! play with temperature etc. in different sessions asking the same question
        - compare results

- context matters (last session RACCE prompt design)
  - now: context via IDE!
  - VSC tour
  - create project for course
    - init with data file from submissions

- ! autocompletion task
  - [session-2.handson.md](session-2.handson.md)
  - upload/submit your created `README.md`

- ? what did happen? what information is used to generate the answer?
  - current file
  - ALL OPEN files
  - AI guide files (AGENTS.md, .github/copilot-instructions.md, https://code.visualstudio.com/docs/copilot/getting-started#_step-4-personalize-your-ai-experience)
  
- ? what is the problem in our setting?
  >> private data was sent online! privacy issues relevant for a lot of things!
  - ? how to avoid?
  
- ? how to ensure privacy when using AI?
  - local vs. cloud service
  - free vs. payed plans
  - privacy settings in tools https://paulsorensen.io/github-copilot-vscode-privacy/
  - separating sensitive data/code from ai-supported projects
    - YOU have to take care when AI is enabled or data leaks are possible

- https://code.visualstudio.com/docs/editing/ai-powered-suggestions

# 3 - pre self-study


# session 3 - "IDE-internal agent mode"

- so far chat or auto-completion: today "IDE-internal agent mode"
  - chat interfaces of VSC
  - https://code.visualstudio.com/docs/chat/chat-overview

- differences to normal chat or autocompletion:
  - access to all files
  - larger context (autocompletion uses only current file; chat only what's given)
  - able to change multiple files in one prompt/task
  - integration into VSC allows to automate also IDE-related tasks

### chat modes:

- inline chat:
  - similar to autocompletion but guided and larger changes possible
  - changes only in current file
  - context = current file
  * show prompt to extend/rewrite column list in README.md
  
- INSPECT CHANGES
  - the diff dialog "Keep"/"Undo" 
  - extend prompt to update current changes

> Task A - [session-3.handson.md](session-3.handson.md)

- chat view
  - context of a prompt can be set (open/selected) and extended (context menu "Add File to Chat")
    - default = current file or selection
    - additional files can be added
    - context definition via `#...`, e.g. `#codebase`, `#readFile`, ..
    - chat partners via `@...`, e.g. `@vscode`, `@codebase`, ...
    - chat commands
      - `/explain`, `/fix`, ...
      - `/compact` - the context problem "solution"

> Task B - [session-3.handson.md](session-3.handson.md)

- next level for our "project":
  - we want to create a nice website that shows our table data
  - to this end do a step-by-step approach (don't use all tasks in one prompt!)
  
> Task C - [session-3.handson.md](session-3.handson.md)

- ? what did you observe? how well did the AI understand your data and documentation needs?
- ? how do you like the different chat modes? when would you use which one?
- ? what are advantages/disadvantages of the different modes?

> Upload/submit your created `index.html` file along with its CSS file!


# self-study material for session 4

- [../episodes/ai-risks-responsibilities.md](Risks, Drawbacks and Responsibilities with AI Usage)


#  session 4

- how to stay in control?
  - have a plan and break it down into small steps

- small, iterative steps
  - allows to check results (get explanations) and adjust prompt
  - allows to stay in control and avoid unwanted changes

- ? how to get a good plan?
  - use an AI chat to get an idea how to do the next step
  - OR use the "Plan"-Agent of VSC to get a step-by-step plan for your task
    - https://code.visualstudio.com/docs/agents/agent-types/local-agents
    - switch to "Plan"-Agent and ask for a plan to create a nice website for our data

> Task A - [session-4.handson.md](session-4.handson.md)


- how to provide bug information from the browser to the AI?
  - open the browser's developer tools (F12)
    - "Console" tab shows errors and warnings
  - copy the error message and provide it to the AI in a new prompt


> Task B - [session-4.handson.md](session-4.handson.md)


- something went wrong?! the timeline feature of files in VSC
  - "timeline" view of file changes
  - "compare with previous version"
  - "revert changes"

> Task C - [session-4.handson.md](session-4.handson.md)

- next level: git-based version control (commit, push, pull, revert, branches, ...)
  - concept of branches and pull requests allows to separate "AI experiments" from main codebase and only merge when satisfied with results
  - next-next level: online git repositories (github, gitlab, bitbucket, ...)
    - bonus: GitHub Copilot operates also in GitHub's web-based code editor and pull request interface, allowing to use AI support also in online code reviews and pull request management



# self-study material for session 5

- https://www.uni-koblenz.de/de/bildungswissenschaften/oer/oer-und-ki/ki-und-urheberrecht
- https://www.uni-koblenz.de/de/bildungswissenschaften/oer/oer-und-ki/oer-erstellen-mit-ki (beispielhafte Anwendung und Verdeutlichung der Urheberrechtsproblematik)


# session 5 - AI-supported work and copyright issues



# Kurzzusammenfassung: Urheberrecht & KI im Programmierkontext

## ⚖️ Die Rechtliche Lage (Stand 2026)

* **Das Schöpferprinzip (§ 2 Abs. 2 UrhG):** Nur Menschen können Urheber sein. Rein maschinell per Prompt erzeugter Code, Text oder Bildinhalt ist **urheberrechtlich schutzlos** (gemeinfrei) und darf von jedem kopiert werden.
* **Der menschliche Beitrag entscheidet:** Ein bloßer Befehl („Schreibe mir JavaScript für...“) reicht nicht für einen Schutz aus. Erst wenn Studierende den KI-Code aktiv anpassen, mit eigenen Ideen kombinieren und strukturieren, kann ein geschütztes Gesamtwerk entstehen.
* **Nutzungsrechte vs. Urheberrecht:** Die AGB der Anbieter (OpenAI, Microsoft) erlauben zwar die freie Nutzung der Ergebnisse, können den Nutzer:innen aber kein gesetzliches Urheberrecht garantieren, wo laut Gesetz keines existiert.
* **EU AI Act (In Kraft ab August 2026):** Es gilt eine gesetzliche Kennzeichnungspflicht für KI-generierte Inhalte (insb. Texte/Bilder) bei Veröffentlichungen. Reiner Programmcode ist davon meist ausgenommen, die sichtbaren Inhalte einer Website jedoch nicht.
* **Das Lizenz- & Haftungsrisiko:** KIs wurden mit geschütztem Open-Source-Code trainiert und können diesen in seltenen Fällen eins zu eins reproduzieren (*Regurgitation*). Das rechtliche Risiko bei Urheberrechtsverletzungen tragen die Anwender:innen, nicht die KI-Anbieter.

---

## 💬 Leitfragen für die vorgeschlagene Kursdiskussion

* **Frage 1 (Kopierschutz):** > *„Ihr habt gerade eine interaktive Website gebaut, ohne eine Zeile JavaScript selbst schreiben zu können. Wenn ein anderes Team eure Website eins zu eins kopiert – könnt ihr euch rechtlich dagegen wehren?“*
* **Kernantwort:** Nein, für den reinen KI-Code nicht. Ein rechtlicher Schutz greift nur für eure eigenen, selbst erhobenen Daten oder für Code-Teile, die ihr massiv selbst modifiziert habt.


* **Frage 2 (Haftung im Ernstfall):** > *„Wer haftet, wenn das JavaScript der KI eine Funktion nutzt, die jemand anderes urheberrechtlich geschützt hat (z. B. aus einem kommerziellen Projekt kopiert wurde)?“*
* **Kernantwort:** Ihr als Anwender:innen tragt das Risiko. Microsoft oder OpenAI haften in ihren kostenlosen Plänen nicht dafür. Ihr seid als „Human-in-the-Loop“ die finale Kontrollinstanz.
