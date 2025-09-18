# 📘 A Beginner’s Guide to OmegaT: Your First Translation in 20 Minutes

> **Note:** This guide shows Windows screenshots. macOS/Linux steps are described without images.

## 1. Introduction

### 1.1. What is OmegaT?
OmegaT is a free, open-source Computer-Assisted Translation (CAT) tool. It stores your translations in a Translation Memory (TM), so repeated or similar text is suggested automatically. This ensures speed and consistency.

### 1.2. Who is this guide for?
- Freelance translators seeking an affordable CAT tool.
- Students learning translation workflows.
- Small teams managing multilingual projects.

No prior knowledge of OmegaT is required.

### 1.3. What you will accomplish
By the end of this guide, you will have:
- Installed and launched OmegaT.
- Created a translation project.
- Translated a short text.
- Exported your finished translation.

**Estimated time:** ~20 minutes.

---

## 2. Prerequisites

### 2.1. System requirements
OmegaT runs on Windows, macOS, and Linux. It requires Java.

- **Windows:** 7, 10, or 11  
- **macOS:** 10.12 Sierra or later  
- **Linux:** Most modern distributions

Check Java by typing `java -version` in Command Prompt/Terminal. If not installed, download OmegaT **with JRE**.

### 2.2. Downloading OmegaT
1. Go to <https://omegat.org>.  
   *(Screenshot: OmegaT homepage with Download highlighted)*
2. Click **Download**.
3. Choose the latest stable version.
   - **Windows:** select **With JRE** if Java is not installed.
   - Otherwise, use the **Without JRE** package.  
   *(Screenshot: Download page with file options highlighted)*

---

## 3. Installation

### 3.1. Windows
1. Locate the downloaded `.exe`.
2. Double-click to run and follow the wizard (default settings recommended).  
   *(Screenshot: Windows installer wizard)*

### 3.2. macOS
1. Open the downloaded `.dmg` file.
2. Drag the OmegaT icon to the **Applications** folder.  
   *(Screenshot placeholder: macOS drag-and-drop installer)*

### 3.3. Linux
- Install from your package manager (`sudo apt install omegat`), or
- Download the `.zip`, extract it, and run the `OmegaT` script.  
  *(Screenshot placeholder: Linux terminal installing OmegaT)*

---

## 4. The OmegaT Workspace
When you launch OmegaT, the main workspace opens.

- **Editor (center):** segments to translate.
- **Fuzzy Matches (top right):** suggestions from TM.
- **Glossary (bottom right):** terminology entries.
- **Project Files (left):** documents in your project.

*(Screenshot: OmegaT workspace with panels labeled)*

---

## 5. Creating Your First Project

### 5.1. Project folder structure
OmegaT creates folders automatically:
- **/source/** – original files.
- **/target/** – translated files.
- **/tm/** – translation memories.

*(Screenshot: OmegaT project folder structure in file explorer)*

### 5.2. Create a new project
1. Go to **Project → New…**.  
   *(Screenshot: Project menu with New highlighted)*
2. In **Project Folder**, create `My First Project`.  
   *(Screenshot: New Project dialog with folder path highlighted)*
3. Confirm the **Project Name**.  
   *(Screenshot: Project Name field)*
4. Set **Source Language** (e.g., English) and **Target Language** (e.g., German).  
   *(Screenshot: Source/Target fields highlighted)*
5. Click **Finish**.

---

## 6. Translation Workflow

### 6.1. Add a source file
1. Create a test file (`test.txt`) with 2–3 English sentences.
2. Save it, then move it into the project’s **/source/** folder.
3. In OmegaT, select **Project → Reload**.
4. Your file appears in **Project Files**. Double-click to open.  
   *(Screenshot: Project Files pane with `test.txt`)*

### 6.2. Translate a segment
1. Click the first segment in the **Editor**.
2. Type your translation in the lower field.
3. Press **Ctrl+Enter** (Windows/Linux) or **Cmd+Enter** (Mac) to confirm and move to the next segment.
4. Repeat until all segments are translated.  
   *(Screenshot: Editor pane with source and target fields labeled)*

### 6.3. Translation Memory and Glossary basics
- Confirmed segments are stored automatically in TM.
- Repeated text shows up as a **100% match**.
- Similar text appears as a **fuzzy match** in the **Fuzzy Matches** pane.  
  *(Screenshot: Fuzzy Matches pane with example match)*

---

## 7. Finalizing and Delivering

### 7.1. Generate translated files
1. Go to **Project → Create Translated Documents**.
2. OmegaT saves the translated file in **/target/**.  
   *(Screenshot: Project menu with Create Translated Documents highlighted)*

### 7.2. Verify output
1. Open the **/target/** folder.
2. Open your translated `test.txt`.
3. Review the content.  
   *(Screenshot: Target folder with `test.txt` highlighted)*

---

## 8. Next Steps
- Try translating a `.docx` file.
- Add an existing Translation Memory.
- Explore glossaries for terminology management.
- See **Help → Documentation** or join the OmegaT support forum.

---

## 9. Glossary
- **CAT Tool:** software that assists translators by storing and reusing translations.
- **Segment:** a sentence or unit of text handled individually in OmegaT.
- **Translation Memory (TM):** database of source text and its translations.
- **Fuzzy Match:** a partial match from the TM (e.g., 75%).
- **Glossary:** approved terms with translations for consistency.
