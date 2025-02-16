# Digital Document Locker

## Overview
The Digital Document Locker is a secure system that allows users to store, manage, and access their important documents digitally. It provides functionalities for user registration, authentication, and document management, including adding, viewing, and deleting documents.

## Features
- **User Signup & Authentication**
  - Secure user registration with password validation.
  - Login with captcha-based authentication.
- **Document Management**
  - Add, delete, and view personal and official documents.
  - Categories include Aadhaar card, PAN card, passport, property papers, bank details, etc.
- **Secure Storage**
  - User credentials and document details are securely stored in binary files.

## Classes and Functions

### 1. `signup` Class
- Handles user registration.
- Stores user credentials securely.
- Ensures strong password policy.

### 2. `Login` Class (Inherits from `signup`)
- Handles user authentication.
- Uses captcha verification to prevent automated logins.

### 3. Document Management Classes
- `twelve`, `pan`, `drive`, `aadhar`, `propertypaper`, `passport`, `bank`
  - Each class manages specific document types.
  - Provides functions to add, delete, and view documents.
- `view`, `viewofficial`
  - Used to display personal and official documents.
- `personaldoc`, `officialdoc`, `adddoc`
  - Used to add personal and official documents.
- `deletedocument`
  - Allows users to delete selected documents.

### 4. Main Functions
- `document()`
  - Displays the main menu for document management.
- `start()`
  - Displays a welcome message and clears the console.
- `main()`
  - Entry point of the program.
  - Initializes the system and continuously handles user input.

## How to Run
1. Compile the program using g++:
   ```sh
   g++ -o document_locker main.cpp
   ```
2. Run the executable:
   ```sh
   ./document_locker
   ```

## Dependencies
- C++ Standard Library
- File handling support

## Future Improvements
- Implement encryption for stored documents.
- Add a graphical user interface (GUI) for better user experience.
- Integrate cloud storage for remote access.

## Contributing
If you’d like to contribute, feel free to fork the repository and submit a pull request.

## License
This project is open-source and available under the MIT License.

