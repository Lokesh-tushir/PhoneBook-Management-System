📞 File-Based Contact Book
A simple and efficient command-line (CLI) contact management system built in Python.

This project allows you to create, view, search, update, and delete contacts. All contact information is saved locally in a contacts.json file, so your data is persistent and saved even after you close the program.

✨ Core Features
Add Contact: Save a new contact with their name, phone number, and email.

View All Contacts: Get a complete, neatly formatted list of all contacts.

Search Contact: Find contacts by name. The search is case-insensitive and matches partial names.

Update Contact: Modify the phone or email of an existing contact.

Delete Contact: Remove a contact from your book.

Persistent Storage: All contacts are saved to contacts.json, so your data is never lost.

Error Handling: Safely handles cases where the contacts.json file is missing or corrupted, starting fresh without crashing.

🛠️ Technologies Used
Language: Python 3

Data Storage: JSON (using Python's built-in json module)

🚀 Getting Started
Follow these instructions to get a copy of the project up and running on your local machine.

Prerequisites
You must have Python 3 installed on your system. To check your version, open your terminal and run:

Bash

python --version
# or
python3 --version
Installation & Running
Clone the repository (or download the files) to your local machine:

Bash

git clone https://github.com/your-username/your-repository-name.git
Navigate to the project directory:

Bash

cd your-repository-name
Run the application:

Bash

python main.py
(Note: You may need to use python3 main.py depending on your system setup. Assumes your file is named main.py)

📋 How to Use
Once the script is running, you will see the main menu. Simply type the number of the option you want and press Enter.

--- File-Based Contact Book ---
1. Add a new contact
2. View all contacts
3. Search for a contact
4. Update a contact
5. Delete a contact
6. Exit
Enter your choice (1-6):
1. Add a new contact: Prompts you to enter a name, phone, and email for the new contact.

2. View all contacts: Displays all currently saved contacts.

3. Search for a contact: Asks for a name to search for. It will show all contacts whose name contains your search term.

4. Update a contact: Asks for the exact name of the contact to update. You can then enter a new phone and/or email. Pressing Enter without typing anything will keep the old information.

5. Delete a contact: Asks for the exact name of the contact you wish to delete.

6. Exit: Saves all changes and closes the program.

📁 How It Works
This program is built around two key functions that handle data:

load_contacts(): This function is called when the program first starts. It tries to open and read the contacts.json file. If the file doesn't exist (FileNotFoundError) or is empty/corrupted (JSONDecodeError), it simply returns an empty list [] so the program can start fresh.

save_contacts(contacts): This function is called every time a change is made (add, update, or delete). It takes the current list of contacts and overwrites the contacts.json file with the new, updated data, ensuring no data is lost.

The main() function contains a while True loop that keeps the menu running until the user decides to exit.

🤝 How to Contribute
Contributions are welcome! If you have ideas for new features or find a bug, feel free to:

Fork the repository.

Create a new branch (git checkout -b feature/YourAmazingFeature).

Commit your changes (git commit -m 'Add some AmazingFeature').

Push to the branch (git push origin feature/YourAmazingFeature).

Open a Pull Request.

You can also just open an issue with the tag "enhancement" or "bug".

📜 License
This project is licensed under the MIT License - see the LICENSE.md file (if you have one) for details.
