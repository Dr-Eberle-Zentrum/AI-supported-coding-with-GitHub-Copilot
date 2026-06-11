Guten Tag, everyone! Welcome to today's hands-on session.

Up until now, you've probably used AI like ChatGPT by typing a prompt, hitting enter, and waiting for a large block of text to come back. Today, we are going to experience a completely different flavor of AI assistance: **inline autocompletion** right inside your code editor, Visual Studio Code (VS Code), using GitHub Copilot.

Think of it like the predictive text on your smartphone, but on absolute steroids. It tries to guess what you want to write before you even finish your thought.

We will use the artificial bank transactions CSV file you prepared earlier. Let’s get our hands dirty!

---

## 🛠️ Step-by-Step Exercise

Follow these five steps to set up your project and see GitHub Copilot in action.

### Step 1: Create a New Project Folder

Before opening VS Code, we need a designated space on your computer for this project.

* Go to your computer's desktop or documents folder.
* Create a brand-new folder and name it `copilot-test`.

### Step 2: Open the Folder and Integrate Your Data

Now, let's open this folder inside Visual Studio Code and add your data.

* Open **Visual Studio Code**.
* Click on **File** in the top menu, then select **Open Folder...** (on Mac, it might just say **Open...**).
* Select the `copilot-test` folder you just created and click open.
* Now, take your artificial bank transactions CSV file from your computer and **drag and drop** it directly into the left-hand sidebar (the File Explorer) of VS Code.

### Step 3: Inspect Your Data Set

Let's make sure VS Code can read your file properly.

* In the left sidebar of VS Code, click once on your CSV file to open it.
  * When clicking on a word in the file, all occurrences should be highlighted..
* Take a close look at the top row (the headers). 
  * *Keep a mental note of these column names!* GitHub Copilot is currently "reading" this file in the background to understand your project context.

### Step 4: Create a "README.md" File

In the world of software and data, a `README.md` file is the standard homepage or instruction manual for any project. 
The `.md` stands for Markdown, which is just a simple way to format text.
If you are not familiar with Markdown yet, here is the [Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/) to look up things.

* Hover your mouse over the left sidebar (where your CSV file is listed).
* Click the **New File** icon (it looks like a piece of paper with a plus sign).
* Type exactly `README.md` and hit **Enter**. You now have a blank document open.

### Step 5: Trigger GitHub Copilot (The Magic Moment)

Now, let’s see the AI work its magic without you having to ask it a direct question.

* Click into your blank `README.md` file and type the following heading exactly:
```markdown
# Bank Transactions Data Documentation

```


* Press **Enter** to go to a new line.
* Now, type the words: **"This data set contains"** and then **STOP typing.** Do not hit enter. Just wait for 2 seconds.

> 💡 **What to look for:** You should see light grey text appear right in front of your cursor. GitHub Copilot has looked at your CSV file, realized what columns are inside it, and is now trying to finish your sentence for you!

* **How to accept it:** 
  - If you like what the AI suggested, simply press the **Tab** key on your keyboard. The **whole** grey text will turn solid, meaning you've accepted the suggestion.
  - If you press **CTRL + Right Arrow** (or **CMD + Right Arrow** on Mac), you can accept the suggestion word by word instead of all at once.
  - When hovering with your mouse over the grey text, you can also see a menue to switch to alternative suggestions and to see the options from above.
* Press **Enter** again and start typing another sentence, like **"The columns included are:"** and wait again. 
* Check whether the suggested names match your exact column names!

---

## 🧠 Why is this different from a Chatbot?

| Feature | Chat-Based AI (e.g., ChatGPT) | Inline Autocompletion (GitHub Copilot) |
| --- | --- | --- |
| **Workflow** | You have to copy-paste data, switch windows, write a prompt, and wait. | It stays quietly in the background right where you are already working. |
| **Context Awareness** | It only knows what you explicitly paste into the chatbox. | It automatically "reads" the other files open in your editor to guess your next move. |
| **Speed** | Takes 10–30 seconds to generate a full response. | Anticipates your next words in **milliseconds** as you type. |

---

### Quick Check-In

Were you able to see the grey text suggestions appear? If the Tab key isn't working for you, or if the grey text isn't showing up, raise your hand and we will come around to check your Copilot activation status!


### 🚀 Next Steps

- Try writing a few more sentences in your `README.md` file and see how Copilot tries to help you.

- Check the Tutorial [Inline suggestions from GitHub Copilot in VS Code](https://code.visualstudio.com/docs/editing/ai-powered-suggestions)
  for more tips and tricks on how to make the most out of GitHub Copilot's inline suggestions.

