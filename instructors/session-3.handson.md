
# 📖 Hands-on Exercise for Session 2: From Typing to Talking – Copilot Chat in VS Code

## 1. Recap: What did we learn?

In our last session, you witnessed GitHub Copilot completing your sentences as if by magic (**Autocompletion**). The secret behind this: the AI quietly reads your open files (like your CSV data) in the background and guesses the most likely next text. You don’t have to prompt the AI explicitly—it simply thinks along with you.

---

## 2. Preparation: Three Ways to Chat in VS Code

In our next session, we want to actively ask the AI questions without ever leaving VS Code. To do this, there are three different ways to open a chat interface. Try out these three keyboard shortcuts in your VS Code before our next class:

### 🗺️ The 3 Chat Types at a Glance

| Chat Type | Shortcut (Windows) | Shortcut (Mac) | When to use it? |
| --- | --- | --- | --- |
| **1. Inline Chat** | `Ctrl` + `I` | `Cmd` + `I` | Directly inside your document to edit or generate a specific line. |
| **2. Chat View** | `Ctrl` + `Alt` + `I` | `Cmd` + `Ctrl` + `I` | In the sidebar for big questions, explanations, or long conversations. |
| **3. Quick Chat** | `Ctrl` + `Shift` + `Alt` + `L` | `Cmd` + `Shift` + `I` | A small search bar at the top for a quick question on the fly. |

---

## 3. Your Session Task: From CSV to HTML

Open your VS Code project from the last session (containing your bank CSV and the `README.md` file).

### Task A: Try out the Inline Chat

1. Open your CSV file
2. Click into the first line containing the CSVs column names
3. Click on the **speech bubble icon** (or `Ctrl` + `I` | `Cmd` + `I`) to open the Inline Chat
4. Request a rewrite of the column names in German or English (whatever it is not right now)


**Observation:** The AI generates the changes and you can review and compare the changes to the old version.

5. Accept the changes if you are happy, otherwise keep on prompting.


### Task B: Refining Your CSV with Inline Chat

Now, let's continue working on your CSV file to make it even better.

* Use the **Inline Chat** (`Ctrl` + `I`) directly in your CSV file.
* Make a second request to refine a specific column name—ask the AI to make it more descriptive or change it to a different language.

> 💡 **Pro Tip:** You can keep refining until you're happy with the result. Each new prompt builds on the previous context!

---

### Task C: Update Documentation via Chat View

Let's now use the **Chat View** for bigger questions that require longer conversations.

#### Step 1: Update Your README.md

* Open your `README.md` file in VS Code.
* Switch to the **Chat View** (`Ctrl` + `Alt` + `I`).
* Request that the AI update your README documentation to reflect the changes you just made to your CSV file.

> 💡 **What the AI will do:** It will read both your CSV and README files in the background and provide updated documentation that matches your new structure.

#### Step 2: Add a New Classification Column

* Still in the **Chat View**, make another request: ask the AI to create a new column that classifies all transactions into **5 reasonable classes** (for example: "Groceries", "Transport", "Entertainment", "Utilities", "Other").
* Request that the AI also update your `README.md` file to document this new column.

---

## 🎯 Project Work: Creating an Interactive HTML Dashboard

Now for the fun part! Let's bring your data to life with a visual representation.

### Step 1: Generate an HTML File

* In the **Chat View**, request a new file called `index.html` that simply and cleanly displays your bank transaction table data as a static page.
* Keep the request straightforward—focus on displaying the data clearly without interactive features for now; we'll add styling later.

### Step 2: Inspect and Test Your HTML

* Once the file is created, open it in a web browser to see how it looks.
  * **Option A:** Double-click the `index.html` file in VS Code's File Explorer to open it in your default browser.
  * **Option B:** Use VS Code's built-in browser by clicking the split-view icon in the top right of the editor.
* Browse through the HTML code in VS Code and take note of any constructs you don't recognize.

### Step 3: Learn About Unknown HTML Elements

* Highlight any HTML tag or code snippet you don't understand (for example: `<table>`, `<thead>`, etc.).
* Use the **Chat View** with the `/explain` command (type `/explain` at the start of your chat message) to get clear explanations of what that code does.
* If you are familiar with HTML, double check the generated code for any errors or improvements you can suggest to the AI. How good is the AI at writing HTML? Can you spot any mistakes or areas for improvement?

### Step 4: Request Styling Improvements

* Take a moment to think about how you'd like your HTML page to look. Do you want:
  * Different colors?
  * Better spacing or fonts?
  * A cleaner layout?
  * Specific lines/borders in the table?
  * Some explanatory text above the table?

* Use either:
  * **Inline Chat** (`Ctrl` + `I`) if you're familiar with HTML and want to make quick edits directly in the code.
  * **Chat View** if you prefer describing your desired changes in plain language and letting the AI handle the implementation.

### Step 5: Separate Styling from Content

* Request that the AI refactor your project by moving styling information into a separate `style.css` file, keeping your `index.html` clean and focused on content only.
* After the changes are made, verify that your HTML file still renders the same in the browser.

> 💡 **Why this matters:** Separating styling from content is a best practice in web development—it makes your code more maintainable and reusable!



---

## 🎯 Food for Thought:

Given the choice: In which situations would you prefer using *Autocompletion*, and when does a *real chat conversation* with the AI make more sense?

