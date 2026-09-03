# Canvas QTI Quiz with ChatGPT4o

Follow these steps to turn your bulk questions, answer choices, and feedback into a Canvas‑ready QTI file—all in one go.

<aside>
<img src="https://app.notion.com/icons/bookmark-outline_lightgray.svg" alt="https://app.notion.com/icons/bookmark-outline_lightgray.svg" width="40px" />

**This page**

[🔹 **Step 1: Prepare Your Raw Quiz Content**](https://app.notion.com/p/Step-1-Prepare-Your-Raw-Quiz-Content-1d9cd88f5bfd8055804cf8b09b7c88d0?pvs=21) 

[🔹 **Step 2: Copy + Paste The Prompt**](https://app.notion.com/p/Step-2-Copy-Paste-The-Prompt-1d9cd88f5bfd809c887edf20244f8949?pvs=21) 

[🔹 **Step 3: Receive Formatted Output**](https://app.notion.com/p/Step-3-Receive-Formatted-Output-1d9cd88f5bfd809cbf23cd0e1e580a0e?pvs=21) 

[🔹 **Step 4: Receive Formatted Output**](https://app.notion.com/p/Step-4-Receive-Formatted-Output-1d9cd88f5bfd80f3a6def200cad4b0da?pvs=21) 

[🔹 **Step 5: Copy & Save**](https://app.notion.com/p/Step-5-Copy-Save-1d9cd88f5bfd808391edcd7981c5ed95?pvs=21) 

[🧩 **Tips & Reminders**](https://app.notion.com/p/Tips-Reminders-1d9cd88f5bfd807a9095d4bc71dc5b6f?pvs=21) 

</aside>

### 🔹 **Step 1: Prepare Your Raw Quiz Content**

Organize everything in plain text, exactly as you’ll paste it. Be sure to include:

1. **Quiz title** and **Quiz description** up front.
2. For each question:
    - **Title:** a short label for your own reference
    - **Points:** positive integer (e.g., 1 or 1.5)
    - **Question text**
    - **All answer choices**, labeling “a)”, “b)”, etc.
    - **Mark the correct choice** by prefixing its line with
    - **Write feedback for every choice**, each on the line immediately after, prefixed with `...`

### 🔹 **Step 2: Copy + Paste The Prompt**

<aside>
🔥

Converting your quiz into QTI involves multiple steps. To save time we’ll let the agent do the heavy lifting, 

</aside>

Copy and paste the following prompt into the chat:

```
Create a quiz to forward to an Educational Designer for importing into Canvas.
Help instructors create Canvas‑compatible quizzes by producing plain‑text files in the text2qti (QTI v1.2) format.

## Step 1. Elicit User Input
- Ask  the user to copy and paste their entire quiz content (paste all questions, choices, and feedback at once) into the chat. There is no need to provide any other information in this initial response.

When the user has inputed their quiz complete the remaining steps.

## Step 2. Gather quiz metadata
- If not present, ask the user to provide the following:
   - Quiz title  
   - Quiz description  

## Step 3. For each question analyse the user input and find:  
- **Question Title** (plain text)  
- **Points** (positive integer or half‑integer)  
- **Question text**  
- **All answer choices**, labeling them “a)”, “b)”, etc.  
- **Which choice is correct**, marked with an asterisk `*` at the start of its line.  
- **General feedback for every choice**,  

## Step 4. Transformation
- Convert all inputs into **text2qti** syntax, embedding the title and points before the numbered question.  
- Use `[ ]` / `[*]` notation for MRQs, 
- Correct answers are indicated a leading "*"
- Follow the example output below exactly:

<example>
Quiz title: Addition
Quiz description: Checking addition.

Title: An addition question
Points: 2
1.  What is 2+3?
a)  6
... Feedback for this particular answer.
b)  1
... Feedback for this particular answer.
*c) 5
... Feedback for the correct answer.
</example>

## Step 5. Final output
- First, output this note (outside of any code block):
"**⚠️ Note:** Copy and paste the text below into a Word document (or plain‑text editor) and save it as a .txt file with Unicode (UTF-8) encoding."
- Immediately after that note, output the entire quiz—including title, description, and all questions—in a single plain‑text code block in the required format.  
**Always**
- Validate numbering, lettering, title and points placement, and asterisk usage against the text2qti specification.
- Keep the note and the quiz strictly separated: the note goes *before* the code block.  
- Prompt for clarification if any required detail is missing.
```

Hit Enter to submit.

### 🔹 **Step 3: Receive Formatted Output**

ChatGPT4o will parse your content and return either 

1. A request to confirm the information it has parsed from the quiz content you have provided. and/or
2. A request to add any missing information. 

You can confirm and/or provide any missing information in the chat and the hit Enter. lo3-mini will convert your quiz into the required format. 

### 🔹 **Step 4: Receive Formatted Output**

ChatGPT4o will return

1. A **note** reminding you to save the text as UTF‑8 `.txt`.
2. A **single code block** containing your complete text2qti quiz (with numbered questions, feedback markers `...`, and correct‑answer asterisks).

---

### 🔹 **Step 5: Copy & Save**

1. **Copy** everything in the code block.
2. **Paste** into a Word document or plain‑text editor.
3. **Save as** “YourQuiz.txt” with **Unicode (UTF‑8) encoding**.
4. **Upload** that `.txt` into Canvas via QTI import.

---

### 🧩 **Tips & Reminders**

- **Title** and **Points** lines must appear **before** the numbered question.
- Always mark the correct option with .
- Prefix **every** feedback line with `...`, even for correct choices.
- No extra formatting—keep it pure plain text. Remove any trailing spaces at the end of lines.

<aside>
<img src="notion://custom_emoji/73f0eb6a-8f02-4281-8295-a2b1c3f67a76/1d0cd88f-5bfd-80da-acb0-007a5c05eebb" alt="notion://custom_emoji/73f0eb6a-8f02-4281-8295-a2b1c3f67a76/1d0cd88f-5bfd-80da-acb0-007a5c05eebb" width="40px" />

Need help with prompts or examples? Contact [**Law Education Design](mailto:stafford.lumsden@sydney.edu.au).**

</aside>