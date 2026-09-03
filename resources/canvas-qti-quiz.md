# Format a Canvas QTI Quiz with ChatGPT 5.4 for Sydney Law School

This guide updates the supplied ChatGPT4o workflow for the current **ChatGPT 5.4 for Sydney Law School** agent. It is designed to help convert bulk multiple-choice or multiple-response quiz material into plain-text **text2qti / QTI v1.2** syntax for later import into Canvas.

## Step 1: Prepare the raw quiz content

Include:

1. **Quiz title** and **quiz description**.
2. For each question:
   - a short **question title**;
   - **points**;
   - the **question text**;
   - all answer choices labelled `a)`, `b)`, etc.;
   - the correct answer(s); and
   - feedback for each answer where required.

## Step 2: Use this transformation prompt

```
Create a quiz to forward to an Educational Designer for importing into Canvas.

Help instructors create Canvas-compatible quizzes by producing plain-text files in the text2qti (QTI v1.2) format.

## Step 1. Elicit user input
Ask the user to paste the complete quiz content, including all questions, answer choices and feedback.

## Step 2. Gather quiz metadata
If not present, ask for:
- Quiz title
- Quiz description

## Step 3. Parse each question
For each question identify:
- Question Title
- Points
- Question text
- All answer choices labelled a), b), etc.
- Which choice is correct
- Feedback for every choice

## Step 4. Transform
- Convert all inputs into text2qti syntax.
- Put Title and Points before the numbered question.
- Use [ ] / [*] notation for multiple-response questions.
- For single-response questions, indicate the correct answer with a leading *.
- Preserve the user's wording unless a formatting change is required.

Example:

Quiz title: Addition
Quiz description: Checking addition.

Title: An addition question
Points: 2
1. What is 2+3?
a) 6
... Feedback for this answer.
b) 1
... Feedback for this answer.
*c) 5
... Feedback for the correct answer.

## Step 5. Final output
First output this note outside the code block:

⚠️ Note: Copy and paste the text below into a plain-text editor and save it as a .txt file with Unicode (UTF-8) encoding.

Then output the complete quiz in one plain-text code block.

Always:
- validate numbering and lettering;
- validate Title and Points placement;
- validate correct-answer markers;
- keep the explanatory note outside the code block; and
- ask for clarification where required information is missing.
```

## Step 3: Review the parsed content

The agent may need you to confirm ambiguous answer keys, question metadata or feedback. Resolve those ambiguities before using the formatted output.

## Step 4: Check the returned syntax

The output should contain:

- the quiz title and description;
- each question in sequence;
- question title and points before the question;
- appropriate correct-answer markers; and
- feedback lines prefixed with `...` where feedback is being used.

## Step 5: Save and import

1. Copy the complete code block.
2. Paste it into a plain-text editor.
3. Save the file as `.txt` using UTF-8 encoding.
4. Pass the file through the established text2qti/QTI import workflow for Canvas.

## Validation reminders

- Check every correct answer marker manually.
- Check that answer order has not changed unexpectedly.
- Check points and question numbering.
- Check multiple-response notation carefully.
- Keep the source quiz as the authoritative version until the imported Canvas quiz has been reviewed.
