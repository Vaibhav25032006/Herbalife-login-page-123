## ✏️ Edit / Update Member Profile

This feature lets existing members update their saved details (name, mobile, email, age, height, weight, gender, fitness goal, and profile photo) without filling a new registration.

### How it works
1. Click **"Update My Details"** on the page, or open the link with `#edit` or `#update` at the end (e.g. `yourpage.html#edit`).
2. Enter your **Member ID** to fetch your saved record.
3. Your existing details auto-fill into the edit form.
4. Change whatever fields you need.
5. Click **Save Changes** — updated data (with recalculated BMI, BMR, TDEE) is sent back to the connected Google Sheet via the Apps Script Web App.

### Setup requirement
- Set `SHEET_WEB_APP_URL` in the script to your deployed Google Apps Script Web App URL.
- The Apps Script backend must handle both `action=search` and `action=update` requests.
- Uploading a new photo is optional — old photo stays if skipped.
