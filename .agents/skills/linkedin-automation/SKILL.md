---
name: linkedin-automation
description: Guidelines and browser automation findings for updating LinkedIn profiles.
---

# LinkedIn Profile Automation Findings

When interacting with a LinkedIn profile using a browser subagent, keep the following technical findings and workarounds in mind to ensure successful execution:

1. **Typing Special Characters (Accents):**
   - Playwright's default keyboard typing (e.g., `browser_press_key`) fails when trying to type special accented characters (like `é`, `à`, `è`), resulting in an "Unknown key" error.
   - **Workaround:** Use `execute_browser_javascript` to directly update the value of text areas or input fields via the DOM (e.g., `document.querySelector('...').value = "..."`). You will likely need to follow up by focusing the field and simulating a manual keystroke (like typing a space) via `browser_press_key` to trigger LinkedIn's React state validation to enable the "Save" (Enregistrer) button.

2. **Handling Modals and Popups:**
   - After saving an experience or section, LinkedIn often opens a confirmation modal (e.g., "Votre expérience est enregistrée" or a Premium upgrade prompt).
   - **Action Required:** You must explicitly wait for and dismiss these modals (by clicking "Ignorer" or the "X" button) before trying to interact with anything else on the underlying page.

3. **Disabled Save Buttons:**
   - If the "Save" button remains disabled after pasting text via JS, select the field, type a single space using the standard input tools, and then backspace it. This fires the necessary keyboard events for LinkedIn's frontend framework to register the change.

4. **Safety Rules (Deleting & Posting):**
   - **NEVER** remove or delete sections from the user's profile.
   - **NEVER** make new posts on the user's timeline.
   - If you believe a section should be removed or cleaned up, do not perform the removal yourself. Instead, **tell the user at the end of your action or ask for explicit confirmation**.
