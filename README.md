📒 Contact Book Web Application
A responsive web app to manage contacts (add, edit, delete) with API key authentication.

(Add a screenshot later if possible)

🚀 Features
View all contacts in a clean table layout.

Add new contacts with name, email, phone, and avatar.

Edit/Delete contacts with confirmation.

API key authentication (stored in localStorage).

Mobile-friendly design with CSS media queries.

🛠 Project Structure
plaintext
project-root/
├── index.html            # Main page (contact list)
├── src/
│   ├── components/
│   │   ├── add-contact.html     # Add new contact form
│   │   ├── edit-contact.html    # Edit contact form
│   │   └── enter-api-key.html   # API key entry page
│   └── config/
├── public/
│   ├── css/
│   │   └── style.css     # All styles
│   └── js/
│       └── config.js     # API key and root path config
├── .gitignore
└── README.md
🔌 How It Works
Authentication:

Users enter an API key in enter-api-key.html.

Valid keys are saved in localStorage via config.js.

CRUD Operations:

Add: Submit form in add-contact.html → POST to API.

Edit: Click a contact in index.html → Pre-filled form in edit-contact.html.

Delete: Confirmation dialog → DELETE request.

Styling:

Responsive design with style.css (flexbox, media queries).

🛠 Setup
Run Locally:

bash
git clone [your-repo-url]
cd contact-book
open index.html  # Or use Live Server in VS Code
API Key:

Open enter-api-key.html first to authenticate.

Dependencies:

None! Pure HTML/CSS/JS.

🔗 Endpoint Reference
Action	Endpoint	Method
Get Contacts	/controller/get-contacts/	GET
Add Contact	/controller/insert-contact/	POST
Edit Contact	/controller/edit-contact/	POST
Delete Contact	/controller/delete-contact/	GET
🐞 Troubleshooting
Links broken? Verify paths match the structure.

API key not saving? Check config.js and browser console for errors.

Styles missing? Ensure CSS paths use ../../public/css/style.css (from src/components/).

📜 License
MIT © [Your Name]

✨ Tips for Enhancement
Add search/filter for contacts.

Use browser storage for offline mode.

Deploy to GitHub Pages/Vercel.

