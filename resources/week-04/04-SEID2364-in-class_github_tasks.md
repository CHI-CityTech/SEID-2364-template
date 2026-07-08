# SEID 2364 — Week 4 In-Class GitHub Tasks (Student Version)

## Purpose

This activity helps you organize your work in a clear and consistent way.

You will:

- convert your assignment into a standard format
- upload it to GitHub
- write short definitions of key ideas

This is not about finding the “correct” answer. It is about making your work clear and easy to follow.

---

## Quick Checklist

Before you finish class, confirm all of these are true:

- I am working in my own branch
- My branch is up to date with `main`
- My folder is named correctly
- My assignment file is named `harm-analysis.md`
- My assignment file is in the correct folder
- My `README.md` includes Ethics, Intelligence, and Harm
- I committed and pushed my changes to my own branch

---

## Folder Structure (Required)

Use this exact structure:

```text
/students/lastname-firstname/
    README.md
    /assignments/
        harm-analysis.md
```

Example:

```text
/students/smith-david/
   README.md
   /assignments/
      harm-analysis.md
```

---

## Before You Begin — Check Your Branch

Make sure you are working in **your personal branch** in the SEID 2364 repository.

- Do not work in the main branch
- Do not upload files to another student’s folder

If you are unsure, ask before continuing.

---

## Before You Begin — Update Your Branch from Main

Before you add or change files, make sure your personal branch includes the latest updates from `main`.

Important:

- You are **not** committing to `main`
- You are bringing the latest course updates from `main` into **your own branch**
- Stay in your own branch when you do your work

If you are using GitHub Desktop:

- Fetch origin
- Make sure your personal branch is selected
- Update your branch from `main`

If you are using the command line:

```bash
git checkout main
git pull origin main
git checkout your-branch-name
git merge main
```

If Git reports a merge conflict, stop and ask for help before continuing.

---

## What is Markdown?

Markdown is a simple way to format text using plain text.

Examples:

- `# Title` → creates a heading
- `## Section` → creates a smaller heading
- `- item` → creates a list

Why we use Markdown:

- It is easy to read
- It works directly in GitHub
- It keeps formatting simple and consistent

You do not need to know all Markdown features. Basic headings and paragraphs are enough.

---

## Markdown vs PDF

### Markdown (for working documents)

- Best for documents you expect to revise over time
- Displays clearly in GitHub and is easy to scan online
- Works well for version control because changes are easier to track
- Good for course work that develops across the semester

### PDF (for fixed documents)

- Useful when layout, pagination, or visual formatting matters
- Good for polished or stable documents that you want to preserve as-is
- Harder to revise and harder to compare across versions
- GitHub preview is more limited than Markdown, especially for navigation and quick reading

In this course:

- Use **Markdown** for documents that are still being developed, revised, or discussed
- Use **PDF** for documents that need a stable visual presentation or fixed layout
- In some cases, keeping **both** is appropriate: Markdown for the working version, PDF for the presentation version
- Choose the format based on the purpose of the document, not just convenience

---

## Task 1 — Convert and Upload Your Assignment

### Step 1 — Find your file

Locate your Assignment 3: Harm Analysis.

This may be:

- Google Doc
- Word file
- or similar

---

### Step 2 — Convert your file

Convert your document to Markdown.

File name must be:

```text
harm-analysis.md
```

Important:

- Do not remove content
- Keep headings and structure
- This is a full conversion, not a summary

For this assignment, use Markdown if you can.

If your document is currently easier to preserve as a PDF, that is acceptable for now, but be careful about the tradeoff:

- Markdown is better when the document will continue to change
- PDF is better when preserving exact layout matters
- If you submit a PDF, make sure it opens clearly in GitHub or can be downloaded easily
- If the assignment becomes a working document later, you may be asked to convert it to Markdown

---

### Step 3 — Go to your folder

Open your personal branch in the SEID 2364 repository.

Go to:

```text
/students/lastname-firstname/assignments/
```

---

### Step 4 — Upload your file

Upload:

```text
harm-analysis.md
```

---

### Step 5 — Check your file

Confirm:

- The file opens in GitHub
- The text is readable
- Headings and spacing look correct
- The file is in the correct folder

If another student cannot read your file easily, it is not correct.

---

## Task 2 — Create a README File

### What is the README for?

The README is the **main page of your folder**.

It serves three purposes:

1. **Entry point**  
   It is the first thing someone reads. It should help them understand your work quickly.

2. **Navigation**  
   It links to your assignments and other materials.

3. **Concept snapshot**  
   It shows your current understanding of key ideas (Ethics, Intelligence, Harm).

Important:

- The README is **short and clear**
- It will be **updated during the semester**
- It is not a full assignment

Think of it as a **dashboard for your work**.

---

### Step 1 — Create the file

Create:

```text
README.md
```

Place it in:

```text
/students/lastname-firstname/
```

---

### Step 2 — Add these sections (Required)

Your README must include:

```md
## Ethics

## Intelligence

## Harm
```

---

### Step 3 — Write your definitions

For each section:

- Write 1–3 sentences
- Be clear and direct
- Use your own words

These definitions are:

- not final
- expected to change later

Avoid:

- very short answers (1 phrase only)
- very long paragraphs
- copying definitions from the internet

Example:

```md
## Ethics

Ethics is the study of how we should act and what responsibilities we have toward others.

## Intelligence

Intelligence is the ability to learn, reason, adapt, and make sense of information.

## Harm

Harm is damage or injury that affects a person, group, or system.
```

---

### Step 4 — Optional (Recommended)

You may add a version line at the top:

```text
Version: Week 4
```

---

### Step 5 — Commit and push

Your folder should now include:

```text
README.md
assignments/harm-analysis.md
```

Example commit message:

```text
Week 4 – Setup and definitions
```

If you are using GitHub Desktop:

- Commit your changes to your personal branch
- Push origin

If you are using the GitHub website:

- Review the file before committing
- Write a clear commit message
- Commit to your personal branch

---

## Key Idea

You are doing two similar things:

- organizing your ideas
- organizing your files

Both require clear structure.

---

## About Privacy

For this course, treat GitHub as a:

### Shared academic workspace

Your work is:

- visible to the class and instructor
- saved over time

We will discuss this more later.

---

## Common Problems

- Wrong folder

  Move the file to `/students/lastname-firstname/assignments/`.

- Wrong file name

  Rename the file to `harm-analysis.md`.

- File does not open correctly

  Re-upload the file and confirm it opens in GitHub.

- Markdown formatting is broken

  Check headings, spacing, and blank lines.

- README is missing sections

  Add `## Ethics`, `## Intelligence`, and `## Harm`.

- Branch is not up to date

  Pull or merge the latest changes from `main` into your branch before continuing.

---

## What Success Looks Like

- Your branch is up to date with `main`
- Your file is complete and readable in GitHub
- Your folder is organized correctly
- Your README includes all required sections
- Your changes are committed and pushed to your own branch

---

## Next Week

We will use:

- GitHub Desktop
- a code editor

This week prepares you for that work.
