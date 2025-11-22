## 📚 Contact Book Python App

This is a simple command-line **Contact Book** application written in Python. It allows users to manage contacts by creating, viewing, updating, deleting, searching, and counting entries stored in a Python dictionary.

-----

## ✨ Features

The application provides a main menu with the following functionalities:

1.  **Create contact:** Add a new contact (Name, Age, Email, Mobile).
2.  **View contact:** Display the full details of a specific contact by name.
3.  **Update contact:** Modify the details of an existing contact.
4.  **Delete contact:** Remove a contact from the book.
5.  **Search contact:** Find contacts whose names match or partially match a search term (case-insensitive).
6.  **Count contacts:** Display the total number of contacts stored.
7.  **Exit:** Close the application.

-----

## 🛠️ How to Run

1.  **Prerequisites:** You must have **Python 3** installed on your system.
2.  **Save the Code:** Save the provided Python code into a file named `contact_book.py`.
3.  **Run from Terminal:** Open your terminal or command prompt, navigate to the directory where you saved the file, and execute the script:

<!-- end list -->

```bash
python contact_book.py
```

4.  **Usage:** Follow the on-screen menu prompts by entering the corresponding number (1 through 7) for the action you wish to perform.

-----

## 💻 Code Structure

The core of the application uses a single **dictionary** to store all contact information:

```python
contacts = {}
```

  * **Key:** The **contact name** (ensuring consistency by using `.strip().title()`).
  * **Value:** A nested dictionary containing contact details: `{'age': int, 'email': str, 'mobile': str}`.

The application runs inside an infinite `while True` loop that continuously displays the menu until the user selects option **7 (Exit)**, which uses the `break` statement to terminate the loop.

-----

## 🛑 Error Handling & Improvements

  * **Input Validation:** Basic `try-except` blocks are used during contact creation/update to ensure the **Age** input is a valid number.
  * **Case Insensitivity:** Search and key lookups convert input to `.lower()` or use `.title()` to handle variations in case when entering or searching for names.
  * **Delete Functionality:** The missing logic for option **4 (Delete contact)** has been fully implemented.

This README should help anyone understand, run, and maintain your Python Contact Book application\!
