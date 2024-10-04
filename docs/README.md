# **ProjectManager**

**Created on**: 2024-10-03

## **Project Description**

The **ProjectManager** is a Python-based tool designed to automate the creation and management of software development projects. It provides an enhanced user experience with the following features:

- **Generate a templated file structure** for different types of projects (Python, Web, or Simple).
- **Automatically create a `README.md` file** with customizable fields such as project name, description, author, and license.
- **Initialize a Git repository** and push the initial commit to GitHub using the GitHub CLI (`gh` command).
- **Metadata tracking** for project details such as version number, start date, and author, saved in a `metadata.json` file.
- **Virtual environment setup**: Optionally create a Python virtual environment for managing dependencies.
- **Manual backup feature** that allows the user to create backups of individual projects with timestamped names.
- **Task tracker and project dashboard**: A simple, visual interface that provides an overview of all projects and their details.

The tool includes a **user-friendly GUI** built with PyQt5, providing an intuitive and professional interface to manage project setup and streamline the creation process.

---

## **Author**

**William Y.**

---

## **Setup Instructions**

1. **Clone the repository**:
   ```bash
   git clone <repo_url>
   ```
2. **(Optional) Set up a virtual environment**:
   ```bash
   python3 -m venv env
   ```
3. **Activate the virtual environment**:
   - On macOS/Linux:
     ```bash
     source env/bin/activate
     ```
   - On Windows:
     ```bash
     .\env\Scripts\activate
     ```
4. **Install dependencies** (if applicable):
   ```bash
   pip install -r requirements.txt
   ```

5. **Run the ProjectManager**:
   ```bash
   python ProjectManager.py
   ```

---

## **Features**

- **Automated project structure generation**:
  Choose from predefined templates for Python, Web, or Simple projects. Creates directory structures such as `src`, `docs`, `tests`, `config`, and more.

- **Customizable README generation**:
  Automatically generate a detailed `README.md` file with project name, description, author, and license information.

- **GitHub integration**:
  Initializes a local Git repository and pushes it to GitHub using the GitHub CLI. Automates the first commit and `git push` to the remote repository.

- **Metadata tracking**:
  Track project version, start date, and other relevant information in a `metadata.json` file for easy reference.

- **Virtual Environment Setup**:
  Create and set up a virtual environment for Python projects to manage dependencies.

- **Manual Backup Feature**:
  Easily create a zipped backup of the project directory, saved in the `Backups` folder with a timestamped name.

- **Task Tracker and Project Dashboard**:
  A PyQt5-based GUI provides a dashboard to view all projects, allowing users to manage projects and track tasks efficiently.

---

## **Project Structure**

Depending on the project type selected, the structure of your project will vary. Below are the folder structures for each template:

### **Python Template**
```plaintext
ProjectName/
├── src/
│   └── modules/
├── tests/
├── docs/
│   └── metrics/
├── assets/
│   └── media/
├── config/
├── logs/
├── scripts/
├── env/
├── build/
└── README.md
```

### **Web Template**
```plaintext
ProjectName/
├── src/
├── static/
├── templates/
├── tests/
├── docs/
└── README.md
```

### **Simple Template**
```plaintext
ProjectName/
├── project/
└── docs/
    └── README.md
```

---

## **Usage**

1. **Launch the GUI**:
   After running the program, a PyQt5 window will appear, allowing you to input your project details:
   - Project Name
   - Template (Python, Web, or Simple)
   - Description
   - Author
   - License
   - Version Number
   - Start Date
   - Option to create a virtual environment

2. **Project Creation**:
   Once you click "Create Project", the tool will:
   - Create the folder structure based on the selected template.
   - Generate the `README.md` file with the provided details.
   - Initialize a local Git repository and push it to GitHub.
   - Create a metadata file (`metadata.json`) with relevant project information.
   - (Optional) Set up a Python virtual environment.

3. **Access your project**:
   Your project will be saved in the following directory:
   ```bash
   /home/riakon/Coding Projects/ProjectName
   ```

4. **Manual Backup**:
   Use the "Backup Project" button from the project dashboard to create a compressed backup of any project.

---

## **Requirements**

- Python 3.x
- Git
- GitHub CLI (`gh` command installed)
- PyQt5
- venv (for virtual environment setup)

---

## **License**

This project is licensed under the **MIT License**.
