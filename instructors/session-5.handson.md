# 📖 Hands-on Exercise for Session 5: Publishing, Copyright, and Version Control

## 1. Context First: Copyright and AI in Programming

Before continuing technical work, we clarify the legal context for publishing AI-supported project results.

## ⚖️ Legal Situation (Status: 2026)

- **Principle of authorship (§ 2 para. 2 UrhG):** Only humans can be legal authors. Code, text, or images created purely by machine prompt are **not protected by copyright** (that is, not eligible for copyright protection and effectively public-domain style in practice) and may be copied by others.

- **Human contribution is decisive:** A simple prompt such as "Write JavaScript for ..." is usually not enough for legal protection. Protection can arise when learners substantially adapt AI output, combine it with their own ideas, and structure it into an original whole.

- **Usage rights vs. copyright:** Provider terms (for example OpenAI or Microsoft) may allow usage of outputs, but terms cannot create statutory copyright if copyright does not exist under law.

- **EU AI Act (in force from August 2026):** There is a legal labeling requirement for AI-generated content (especially text/images) when publishing. Pure program code is usually excluded, but visible website content is generally not.

- **License and liability risk:** AI systems are trained on copyrighted material and may rarely reproduce parts very closely (regurgitation). In practice, legal risk for copyright infringement remains with users, not with AI providers.

---

## 2. Guiding Questions for Discussion

- **Question 1 (Protection against copying):**
	*"You just built an interactive website without being able to write JavaScript on your own. If another team copies your website one-to-one, can you take legal action?"*

	**Core answer:** No, not for purely AI-generated code. Legal protection generally applies only to your own self-collected data or code parts that you have substantially modified yourself.

- **Question 2 (Liability in serious cases):**
	*"Who is liable if AI-generated JavaScript uses a function that is copyrighted by someone else (for example from a commercial project)?"*

	**Core answer:** You, as the users, carry the risk. Microsoft or OpenAI are generally not liable for this in their free plans. As the human in the loop, you are the final control instance.

---

## 3. Your Session Tasks

Continue with the project from previous sessions.

### Task A: AI Check on EU AI Act Notice and Project License

1. Open an AI chat of your choice and ask:
	- whether your website needs an explicit notice for AI-generated code/content to comply with the EU AI Act
	- Ask the AI to justify its answer with legal context and, if possible, references.

2. Let's discuss your insights within the group!

3. Licence your project: 
	- make a preliminary decision on which license to use for the project (and why).
    - Add a license file to your project and update your README.md file accordingly.

---

### Task B: Inspect File History with Timeline

1. Open the **Timeline** view for your `index.html` file in VS Code.

2. Check how many versions are available.

3. Find a version from before a major AI-generated change.

4. Compare it with the current or previous version.

5. Identify what changed and decide which version you prefer.

> 💡 Timeline is especially useful when one file changed in an unexpected way and you want a quick local comparison.

---

### Task C: Discuss and Try Git-Based Version Control

Now move from file-level recovery to project-level safety.

1. Open the **Source Control** view in VS Code.

2. Check whether your project is already a git repository.

3. If it is not, use "Publish to GitHub" to create a new repository and push your project.

4. Experience the following git features in full speed (self-study material linked within the session plan):
    - commit changes
    - create a new branch
    - switch between branches
    - merge branches
    - revert changes

5. Discuss how **commits**, **branches**, and **pull requests** can separate AI experiments from the stable state of your project.

> 💡 Key idea: AI can generate many changes quickly, but git lets you review and integrate them deliberately.


---

### Task D: Publish with GitHub Pages

Now we want to publish our created website that is located within our GitHub repository.
To this end, we want to use the GitHub Pages feature.

Typically, the `index.html` file is located in the root of your repository. 
If you have created a subfolder for your website, make sure to name the respective folder in the GitHub Pages settings done in the following.

1. Open your GitHub repository in a web browser.
2. Click on the **Settings** tab
3. Scroll down to the **Pages** section in the left sidebar.
4. Select the branch you want to publish (usually `main`) and click **Save**.
5. Wait a few minutes and then check the provided URL to see your published website.
6. Update your README.md file to include the URL of your published website.
7. Also enable the GitHub Pages URL in the "About" section of your repository.

The publishing process uses an engine call Jekyll to revise your HTML files. 
In our case, the website is static and does not require any further processing.
Thus, to speedup publishing, we can disable the Jekyll engine by creating a file named `.nojekyll` in the root of our repository.

8. Create a new file in the root of your repository and name it `.nojekyll`.


---

## 🎯 Food for Thought

- Which part felt more challenging today: legal reflection or technical recovery?

- How much AI experimentation feels safe without version control?

- What is your minimum safety and compliance workflow before publishing project results?
