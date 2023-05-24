# Flask Firebase Authentication Application

Welcome to my simple web application built with Flask and Firebase for user authentication. This application allows users to create accounts, sign in to their accounts, manage their profiles, and reset their passwords. It's a great starting point for those interested in implementing Firebase Authentication into their Flask applications.

## Core Features

- **User Registration:** New users can create their own accounts.
- **User Authentication:** Existing users can authenticate into their accounts.
- **Session Management:** The application maintains user sessions to keep the users signed in.
- **Profile Management:** Users can view their profile information.
- **Password Reset:** Users can reset their forgotten passwords.
- **Firebase Integration:** The application integrates with Firebase for back-end services.
- **UI Design:** The application comes with pre-designed user interface for common authentication tasks.
- **Security:** Passwords are securely managed, and sessions are properly handled to avoid common security issues.

## Prerequisites

Before you start, you need to have the following:

- Python (Version 3.6 or above)
- Flask
- Pyrebase (A Python wrapper for the Firebase API)

## Setup Instructions

Follow these steps to get the application running:

1. Clone this repository to your local machine.
    ```bash
    git clone https://github.com/rituraj009/Flask-Firebase-Authentication
    ```

2. Navigate into the project directory.
    ```bash
    cd app
    ```

3. Install the required packages.
    ```bash
    pip install -r requirements.txt
    ```

4. Setup your Firebase project:

    - Navigate to the [Firebase Console](https://console.firebase.google.com/)
    - Create a new Firebase project.
    - Under "Your Apps" in "Project Settings", select the "Config" radio button to get your Firebase SDK config.
    - Replace the "config" variables in `app.py` with your own Firebase project credentials.

    It should look like this:

    ```python
    config = {
    "apiKey": "<your-api-key>",
    "authDomain": "<your-auth-domain>",
    "databaseURL": "<your-database-url>",
    "storageBucket": "<your-storage-bucket>"
    }
    ```
    
    - Enable the Firebase Realtime Database by clicking on Realtime Database in the left panel, and adjust the rules setting to enable read and write access.

    ```json
    {
      "rules": { ".read": true, ".write": true }
    }
    ```

## Running the Application

To start the application, execute the following command in your terminal:

```bash
python app.py
```

## Screenshots
![login](https://github.com/rituraj009/Flask-Firebase-Authentication/assets/102078863/68f50ef8-a3ef-4734-8007-bacdbe9d036f)


Welcome Page for now
![profile](https://github.com/rituraj009/Flask-Firebase-Authentication/assets/102078863/56855b5a-b36c-4f60-9312-96c0b6ca104a)

## Contributing
Contributions are very welcome! Feel free to fork the repository and submit pull requests. If you want to make major changes, please open an issue first to discuss what you'd like to change. If you encounter any issues or have any questions, don't hesitate to open an issue. I appreciate any feedback!

