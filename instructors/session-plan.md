

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

> Task: 
> - rewrite CSV header in German or English
> - use a second prompt to request a specific column name for one column

- chat view
  - context of a prompt can be set/extended
    - default = current file or selection
    - additional files can be added
    - context definition via `@codebase`, `@readFile`, ..
    - chat commands
      - `/explain`, `/fix`, ...
      - `/compact` - the context problem "solution"

> Task: 
> - update header documentation in README.md w.r.t. updated CSV file
> - request the creation of a new column that classifies all transactions into 5 reasonable classes + "other" along with an update of the README.md


- next level for our "project":
  - we want to create a nice website that shows our table data
  - to this end do a step-by-step approach (don't use all tasks in one prompt!)
  
> Tasks:
> - (1) request a new file "index.html" that nicely shows the table data from the CSV file
> - (2) inspect the file 
>    - use either web browser or VSC-internal browser to see the result
>    - browse the HTML code (file content), highlighted unknown constructs and get explanations with `/explain` via chat view
> - (3) think about styling changes you want to have and request them
>    - if you are familiar with HTML use the inline chat, otherwise the chat view
> - (4) request within the chat to revise your index.html and to store styling information separately
>    - check whether the new separated file architecture renders index.html the same in the browser

