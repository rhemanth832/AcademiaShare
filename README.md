**Academia Share – Django-based Campus File Sharing System 📔**

![Academia Share Icon](https://github.com/user-attachments/assets/61c88cd4-42c9-447d-998a-adb6288b0199)


##

**Description**

**Academia Share** is a Django-based Campus Repository designed to streamline the file-sharing process between teachers and students. The platform offers distinct homepages for both teachers and students, each tailored to their specific needs. Teachers can efficiently manage files, set permissions, and maintain control over their uploads. On the other hand, students gain easy access to educational resources and a seamless file search experience.

##

**Features**

### Teacher Homepage

* **Upload Files:**
  Teachers can upload files directly to the repository, making educational materials easily accessible to students. 📤

* **Delete Files:**
  Teachers have the capability to remove files, ensuring content relevance and organization within the repository. 🗑️

* **Set Permission Access:**
  Control file access by setting permission levels. Teachers can manage who can view and download their uploaded files. 🔒

* **File Filtering:**
  Teachers can view only the files they have uploaded, creating a personalized and organized experience. 📂

### Student Homepage

* **View All Files:**
  Students have access to a comprehensive list of all files uploaded by teachers, facilitating easy discovery of educational resources. 👀

* **Download Files:**
  Students can download files uploaded by teachers, enabling offline access to course materials. 📥

* **Search Functionality:**
  An efficient search feature allows students to find files by their names, making it simple to locate specific educational resources. 🔍

##

**Tech Stack**

* **Django:**
  The web application is built using the Django framework, providing a robust and scalable foundation for campus repository management. 🐍

* **Python:**
  The backend logic and functionality are implemented using Python, ensuring a clean and efficient codebase. 🐍

* **SQLite Database:**
  The project utilizes SQLite for database management, offering a lightweight and easily deployable solution. 🗃️

* **HTML/CSS/JavaScript:**
  The frontend is designed using a combination of HTML, CSS, and JavaScript to create a user-friendly and responsive interface. 🌐

##

**Setup**

Step-by-step instructions to set up and run the project.

### Prerequisites

1. **Download Python:**

   * Visit the [Python Download Page](https://www.python.org/downloads/) to download the latest version of Python.
   * Follow the installation instructions for your operating system.

2. **Get Pip:**

   * Pip usually comes bundled with Python installations after version 3.4. If you need to install or upgrade it, follow the instructions on the [Pip Installation Guide](https://pip.pypa.io/en/stable/installation/).

### Project Setup

3. **Install Django:**

   * Open a terminal or command prompt.
   * Clone the file using:
     
   ```bash
     git clone https://github.com/rhemanth832/AcademiaShare.git
     ```
   ```bash
     cd AcademiaShare
     ```
   
   * Run the following command to install Django:

     ```bash
     pip install django
     ```

3. **Install SMTPMail and MIME:**

   * Run the following commands to install the required packages:

     ```bash
     pip install smtpmail
     pip install mime
     ```

4. **Set Absolute URLs for Images: (Optional)**

   * Open `login/views.py` and `teacherhome/views.py`.
   * Locate the URL for `textLogo.png` in both files.
   * Replace the relative URL with an absolute URL. Example:

     ```python
     # Before
     img_url = 'textLogo.png'

     # After
     img_url = 'D:/path/to/the/image'
     ```

5. **Change Gmail and Password (Optional)**

   * Open `login/views.py` and `teacherhome/views.py`.
   * Locate the `MAIL_ID` and `PASSWORD` variables in both files.
   * Change the password and email to your own.
   * Refer here: [Steps to Create App Password – Google](https://support.google.com/accounts/answer/185833?hl=en)

     ```python
     MAIL_ID = "ENTER_YOUR_GMAIL"
     PASSWORD = "xxxx xxxx xxxx xxxx"
     ```

### Database Setup

7. **Run Migrations:**

   * In the root directory of your project, run the following commands to set up the database:

     ```bash
     python manage.py makemigrations
     python manage.py migrate
     ```

### Run the Project

8. **Start the Development Server:**

   * Run the following command to start the development server:

     ```bash
     python manage.py runserver
     ```

   * Visit [http://127.0.0.1:8000/](http://127.0.0.1:8000/) in your web browser to view the project.

##

**User Interface (UI) and Email Client**

![login](assets/login.png)
![signup](assets/signup.png)
![no access](assets/no%20access.png)
![Screenshot 2025-07-06 125450](https://github.com/user-attachments/assets/11f4c743-d00c-4cb3-a798-53257f4ee0d5)
![Screenshot 2025-07-06 125417](https://github.com/user-attachments/assets/043eaf39-a375-4a49-b8e6-01f5867ceaa1)



##

**Getting Started**

To set up and run **AcademiaShare** locally, follow the instructions in the [Project Setup Guide](#) provided in the repository.

##
