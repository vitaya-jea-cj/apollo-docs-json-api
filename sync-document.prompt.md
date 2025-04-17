# Apollo UI Documentation Sync Process

This prompt documents the process for extracting, structuring, and syncing Apollo UI component documentation into JSON files for each component.

## Process Steps

1. **Component List Review**
   - Review the list of components in `components.md` and determine the documentation source for each.

2. **Documentation Extraction**
   - For each component, visit the Apollo UI documentation site (https://cjx-apollo-ui.netlify.app/docs/components/).
   - Extract the following for each component:
     - Description
     - Props (name, type, default, description, required)
     - Examples (title, description, code)
     - CSS classes
     - Migration guide (if available)
     - Source link

3. **JSON Structuring**
   - Structure the extracted data into a JSON object with the following keys:
     - `component`, `id`, `slug`, `description`, `props`, `examples`, `css`, `migrationGuide` (if any), `sourceLink`
   - Use consistent naming and formatting for all fields.

4. **File Creation**
   - Save each component's JSON documentation in the `docs/` directory as `<component>.json` (e.g., `button.json`).

5. **Validation**
   - Ensure all required fields are present and the JSON is valid.
   - Check for consistency in prop types, example formatting, and CSS class documentation.

6. **Repeat**
   - Repeat steps 2–5 for all components in the list.

7. **Update & Maintenance**
   - When Apollo UI documentation changes, repeat the extraction and update the relevant JSON files.

---

This process ensures that the local JSON documentation stays in sync with the official Apollo UI documentation and is structured for easy consumption by other tools or documentation systems.
