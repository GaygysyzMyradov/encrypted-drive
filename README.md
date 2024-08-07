# Encrypted Drive
Encrypted Drive is a robust web application developed with Django, designed to serve as a secure file management system with advanced encryption features. Built using Python Django and utilizing the Fernet encryption library, it provides seamless file upload and download capabilities within a user-friendly environment. Users can trust their data remains confidential and protected with AES-128 encryption.

## NOTE
If you wish to test or use the EncryptedDrive, please follow the link below to access it in the case that you are unfamiliar with GitHub. Thank You! 

[CLICK HERE](https://drive.google.com/file/d/1TJzMfZ9KM4npWd-grNX0wd1Ovm0FiQFZ/view?usp=share_link)

## Key Features
- User Authentication: Ensure user privacy and data integrity with secure log-in and log-out functionalities.

- File Encryption/Decryption: Elevate the security of your files through integrated encryption and decryption features.

- Folder Management: Create and delete folders to organize files more efficiently.

- Sorting and Searching: Easily organize and locate files with intuitive sorting and searching options.

- Download and Upload: Effortlessly manage files by downloading and uploading within the encrypted environment.

## Getting Started
1. Install Python
2. Open the Project
3. Install project with venv. Run the following commands. (If python command is not found, then try python3 command)

```bash
  python -m venv venv
  
  for Windows OS:
   cd venv/scripts/activate
   
  for Linux or MacOS: 
    source venv/bin/activate
```

4. Go to the project folder

```bash    
  pip install -r requirements.txt

  python manage.py runserver
```
5. In the terminal, find a local host link. It should be something like: http://127.0.0.1:8000/

[NOTE]: If there is another application running in the Port :8000, you can specify a port number by running the command:

```bash    
  python manage.py runserver 9000
```

## If you are using MacOS
For MacOS users, while trying to Reset Password, they might face with the following error:

```bash    
  ssl.SSLCertVerificationError: [SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed:
```

To fix it, follow the next steps
1. Open your terminal.
2. Navigate to the System Applications (Not the User Applications) folder where the Python is installed.
3. Run the following commands

```bash    
  cd Python\ 3.11/  //Change the Version to the Version that is installed on your machine
  ./Install\ Certificates.command
```
4. Try resetting your password, the issue should have been solved. 


## Creating a Super User
You can create a Super User to access the Admin Interface
[NOTE] Only one Super User allowed. If you have forgotten your password, you may Reset it on the App Login Page

Follow the commands below. You may set whatever Email or Password you want.
[NOTE] Super Users can also access the Web Application using the same Login Credentials. They can also use the App's Encryption and Decryption features.

```
python manage.py createsuperuser

admin credentials:
email: admin@gmail.com
password : admin
```
