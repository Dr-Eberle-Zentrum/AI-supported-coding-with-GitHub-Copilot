# 📖 Hands-on Exercise for Session 4: Staying in Control

## 1. Recap: What did we learn?

In our last session, you used different chat modes in VS Code to generate and revise content across files.

You saw that AI can speed up documentation and coding tasks, but it can also make broad changes very quickly.

Today, we focus on one key skill: **staying in control** by working in small, verifiable steps.

---

## 2. Preparation: Control-First Workflow

Before you start, keep these principles in mind:

- Work in **small, iterative steps**.
- Check each result immediately.
- Ask for explanations when something is unclear.
- Use browser errors as feedback tools.
- Use VS Code's **Timeline** feature to recover from unwanted changes.
- Git-based workflows are next level safety.

---

## 3. Your Session Task: From Static to Interactive Website

Continue with your existing project from Session 3 (`index.html` + `style.css`).

Your goal is to turn your static website into an interactive one using JavaScript while keeping full control of the process.

### Task A: Create a Plan with the Plan Agent

1. Open the **Chat View** in VS Code.
2. Switch from your default chat mode to the **Plan** agent.
3. Ask for a step-by-step plan to transform your current website into an interactive version using JavaScript.
4. Review the generated plan critically.
5. Adjust the plan so it matches your priorities and skill level.

> 💡 Hint: Ask for explicit milestones (for example: data loading, filtering, sorting, interaction states, error handling).

---

### Task B: Execute the First Plan Step Only

1. Start with **only the first step** of your revised plan.
2. Let the AI implement it (or co-implement it with you).
3. Check whether the feature works as intended.
4. Ask follow-up questions until you understand every relevant code change.

> 💡 Control principle: One change set at a time is easier to validate than one giant AI-generated rewrite.

---

### Task C: Use Browser Errors as AI Input

1. Open your page in a browser.
2. Open Developer Tools (`F12`).
3. Go to the **Console** tab and check for errors or warnings.
4. If any, copy one concrete error message and paste it into a new AI prompt.
5. Ask the AI to fix that exact issue.
6. Re-test and repeat this loop while **extending interactivity** according to your revision plan.

> 💡 Good prompts include: expected behavior, actual behavior, exact error text, and where it appears.

---

### Task D: Recover with VS Code Timeline

If AI changes go in the wrong direction, use VS Code's history features:

1. Open the **Timeline** view for your `index.html` file.
2. Count how many versions are available.
3. Find a version from before a major AI change.
4. Compare with the previous version.
5. Decide whether to keep, partially reuse, or revert changes.

> 💡 This gives you a safety net for experimentation.

---

## 4. Optional Next Level: Git-Based Safety

- [Self-study: Introduction to git and GitHub using GitHub Desktop](https://dr-eberle-zentrum.github.io/intro-to-git-and-github/instructor/01-git-basics.html) (Material of the respective micro course)
- [Quickstart: use source control in VS Code](https://code.visualstudio.com/docs/sourcecontrol/quickstart)

If time allows, we will discuss or try a git-based workflow:

- Keep AI experiments in separate branches.
- Merge only reviewed and understood changes.
- Use pull requests for transparent comparisons.

---

## 🎯 Food for Thought

- Which strategy helped you stay most in control: planning, console-based debugging, or timeline comparison?
- At what point does AI support save time, and at what point is it faster to code manually?
- How can you ensure that final code is still truly **your** code?
