

# session plan


# session 1 - kick-off meeting + chat-based AI support

- who I am and my background

- ? who-is-who?
  + ? AI experiences / usage so far?
  
- ? what are open (AI-related) questions? (optional submission exercise before session?)

- course layout
  - workflow
  - intro to ai-based tests of self-study + code-word submission
  - expectations and what to expect

- ? (how) did your "knowledge search strategy" changed since AIs are available?

- AI in chat-mode for coding
  - discussion on previous experiences
    - ? what platforms used/registered? 
      - allrounder: chatgpt, claude, gemini, ms copilot, deepseek, ... )
      - research: perplexity (with source citations)
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
      - different models selectable


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
  - typically 2-3 model tiers, which differ in
    - input/context size
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
  - free vs. paid plans
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


#  session 4 - "Staying in Control: Small Steps, Testing, and Debugging"

- discussion on responsibilities and risks of AI usage
  - change of roles and focus of the human-in-the-loop
  - test & debug AI-generated code

- how to stay in control?
  - have a plan and break it down into small steps

- small, iterative steps
  - allows to check results (get explanations) and adjust prompt
  - allows to stay in control and avoid unwanted changes

- ? before we start: how many GitHub Copilot Credits are left this month? 
  - check and compare
  - maybe disable autocompletion for a while to avoid unnecessary credit usage

- **Presentation** of current project state (static website with table data)
  - maybe it shows that similar color schemes are used, revealing that the same AI model was used with similar prompts
    - (!) when using AI, be aware that the outcome is not necessarily unique nor original, but can be similar to other users' results
  - ? does all shown tables have a "category" column? if not, how to add it? (see session 3)

- ? how to get a good plan?
  - use an AI chat to get an idea how to do the next step
  - OR use the "Plan"-Agent of VSC to get a step-by-step plan for your task
    - https://code.visualstudio.com/docs/agents/agent-types/local-agents
    - switch to "Plan"-Agent and ask for a plan to create a nice website for our data

> Task A - [session-4.handson.md](session-4.handson.md) - make a plan
> Task B - [session-4.handson.md](session-4.handson.md) - do 1st step and check


- how to provide bug information from the browser to the AI?
  - open the browser's developer tools (F12)
    - "Console" tab shows errors and warnings
  - copy the error message and provide it to the AI in a new prompt


> Task C - [session-4.handson.md](session-4.handson.md) - browser errors as feedback for AI

- **Presentation** of current project state (dynamic website)
  - ? what did you add?
  - ? limitations?
  - ? next steps?

- ! **Reminder** submission of "Food for Thought" reflection till next session


# self-study material for session 5

- https://www.uni-koblenz.de/de/bildungswissenschaften/oer/oer-und-ki/ki-und-urheberrecht
- https://www.uni-koblenz.de/de/bildungswissenschaften/oer/oer-und-ki/oer-erstellen-mit-ki (beispielhafte Anwendung und Verdeutlichung der Urheberrechtsproblematik)


# session 5 - Publishing and Copyright Issues 

- we are now at the point where we want to publish our project
  - ? what are the legal issues when publishing AI-generated content?
    - mention AI-supported content in your README.md file and HTML page (e.g. in a footer) within academic context
  - ? can you claim copyright for your project? who is the author of AI-generated content? 
    - what license to use for your project? (e.g. MIT, Apache, CC-BY-SA, ...)
    - maybe different licenses for different parts of your project (e.g. MIT for code, CC-BY-SA for text and images)
  - ? what about copyright issues? who is responsible for copyright violations?

- EU AI Act (in force from August 2026)
  - legal labeling requirement for AI-generated content (especially text/images)
- ? is the EU AI Act relevant for our project? > check the internet with an AI chat
  - ask whether your website needs an explicit notice for AI-generated code/content
  - discuss the distinction between generated code and visible generated content in published pages
  - ask for legal context and references


> Task A - [session-5.handson.md](session-5.handson.md) - AI check on EU AI Act notice and project license decision

- something went wrong?! the timeline feature of files in VSC
  - "timeline" view of file changes
  - "compare with previous version"
  - "revert changes"

> Task B - [session-5.handson.md](session-5.handson.md) - timeline as recovery tool

- next level: git-based version control (commit, push, pull, revert, branches, ...)
  - concept of branches and pull requests allows to separate "AI experiments" from main codebase and only merge when satisfied with results
  - next-next level: online git repositories (github, gitlab, bitbucket, ...)
    - bonus: GitHub Copilot operates also in GitHub's web-based code editor and pull request interface, allowing to use AI support also in online code reviews and pull request management

> Task C - [session-5.handson.md](session-5.handson.md) - git-based safety and review


> Task D - [session-5.handson.md](session-5.handson.md) - github pages setup


- course wrap-up
  - ? which part felt most challenging? interesting? useful? (technical vs. legal)
  - ? overall feedback? was it worth the time and effort? what would you change for next time?


