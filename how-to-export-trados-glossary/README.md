
# 📘 Export a Bilingual Glossary from Trados Studio

## Who this is for
Translators and project managers who need to share a bilingual glossary created in **Trados Studio** with colleagues or clients.

## What you need before you start
- SDL Trados Studio installed on your computer  
- An existing termbase or project with translation units you want to export  
- Permission to save files to your computer

## Steps

1. **Open your project in Trados Studio.**  
   Launch Trados and select the project that contains the glossary or termbase you want to export.

2. **Go to the Termbase view.**  
   In the top ribbon, click **Termbase** (sometimes called **Terminology**). This opens the termbase connected to your project.

3. **Select the termbase.**  
   In the left panel, highlight the termbase you want to export.

4. **Start the export.**  
   From the top menu, choose **Termbase Management → Export**.

5. **Choose the export format.**  
   - Select **TBX** (TermBase eXchange) if you want a format most CAT tools can read.  
   - Select **CSV** if you prefer a spreadsheet format (openable in Excel).  
   - Select **XML** if the glossary will be imported into another Trados project.

6. **Select the fields to include.**  
   A dialog will let you choose which fields (Source term, Target term, Notes, etc.) you want in the exported file. Tick the boxes you need.

7. **Save the file.**  
   - Click **Browse…** to choose a folder.  
   - Type a file name (e.g., `Glossary_DE-EN.tbx`).  
   - Click **Save → OK**.

## Result
You now have a bilingual glossary file (TBX, CSV, or XML) saved on your computer, ready to share with colleagues or import into other tools.

## If things go wrong
- **I can’t see “Termbase Management.”**  
  → Make sure the termbase is attached to your project. Go to **Project Settings → Language Pairs → Termbases** and add it.  

- **The exported file is empty.**  
  → Check that the termbase actually contains entries. Open it inside Trados to confirm.  

- **The recipient can’t open the file.**  
  → Try exporting to a more universal format (CSV is usually safest).

---

*Last updated: 2 Sept 2025*
