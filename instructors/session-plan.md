

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

# session 2

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


# 3 - self-study

- https://code.visualstudio.com/docs/editing/ai-powered-suggestions
