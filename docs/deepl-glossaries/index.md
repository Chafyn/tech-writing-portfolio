# DeepL — Create and Manage Glossaries

> Learn how to create, populate, and use DeepL glossaries for consistent terminology.

!!! note "Who is this for?"
    Translators and technical writers who need term consistency across projects.

---

## Prerequisites

- DeepL account (Free or Pro)
- Browser access  
- Optional: API key (for the API example)

---

## Create a Glossary

<figure>
  <img src="images/create-glossary.png" alt="DeepL Glossary creation dialog">
  <figcaption>Create a new glossary from DeepL's Glossary panel.</figcaption>
</figure>

1. Open **DeepL** and go to **Glossaries**.
2. Click **New glossary** and provide a name and language pair.
3. Click **Create**.

!!! tip "Naming convention"
    Use a project prefix (e.g., `ACME_UI_en-de`) to keep glossaries organized.

---

## Add Entries

You can add terms one by one, or paste a CSV.

=== "Add Manually"
    1. Click **Add entry**.  
    2. Enter **Source term** and **Target term**.  
    3. Click **Save**.  

    > **Tip:** Add notes in the **Comment** field for edge cases.

=== "Paste CSV"
    Paste lines using this format:

    ```text
    source_term,target_term,comment
    file,Datei,UI label
    folder,Ordner,UI label
    translate,übersetzen,verb form
    ```

    !!! warning "CSV rules"
        - Use **commas** as separators.  
        - No quotes unless a field contains a comma.

<figure>
  <img src="images/add-entries.png" alt="Adding glossary entries in DeepL">
  <figcaption>Bulk entry via CSV paste saves time for larger term sets.</figcaption>
</figure>

---

## Use the Glossary in Translation

- Start a translation as usual.  
- Select your **Glossary** from the dropdown for the current language pair.  
- Terms will be replaced automatically according to your entries.

> **Note:** If a term is not replaced, check the exact **case** and **plural** form.

---

## Export / Import (Reference)

| Action   | Where to click                    | Result                    |
|---------|-----------------------------------|---------------------------|
| Export  | Glossary → ••• → **Export CSV**   | Downloads CSV of entries  |
| Import  | Glossary → **Add entries** → CSV  | Appends entries           |

Footnote example: Glossary behavior may vary slightly across languages[^1].

[^1]: DeepL occasionally updates glossary handling for specific language pairs.

---

## Troubleshooting

??? info "Glossary not visible?"
    - Confirm the **language pair** matches your document.  
    - Refresh the page after creating a new glossary.

??? failure "CSV import failed"
    - Ensure **three columns**: source, target, comment (optional but keep column).  
    - Remove stray semicolons or tabs.

---

## Optional: API Example (Advanced)

If you have an API key, you can create a glossary programmatically.

```bash
curl https://api-free.deepl.com/v2/glossaries \
  -H "Authorization: DeepL-Auth-Key YOUR_API_KEY" \
  -d "name=ACME_UI_en-de" \
  -d "source_lang=EN" \
  -d "target_lang=DE" \
  --data-urlencode "entries=file,Datei\nfolder,Ordner\ntranslate,übersetzen"
