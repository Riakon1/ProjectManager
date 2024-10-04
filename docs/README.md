# **ProjectManager**

**Created on**: 2024-10-03

## **Project Description**

The **ProjectManager** is a Python-based tool designed to automate the creation and management of software development projects. It allows users to:

- **Generate a templated file structure** for different types of projects (Python, Web, or Simple).
- **Automatically create a `README.md` file** with customizable fields such as project name, description, author, and license.
- **Initialize a Git repository** and push the initial commit to GitHub using the GitHub CLI (`gh` command).

The tool includes a **user-friendly GUI** built with Tkinter, allowing users to easily manage project setup while maintaining consistency across different projects.

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

- **GUI interface**:  
  A Tkinter-based GUI for a simple and intuitive project creation process.

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
   After running the program, a Tkinter window will appear, allowing you to input your project details:
   - Project Name
   - Template (Python, Web, or Simple)
   - Description
   - Author
   - License

2. **Project Creation**:  
   Once you click "Create Project", the tool will:
   - Create the folder structure based on the selected template.
   - Generate the `README.md` file with the provided details.
   - Initialize a local Git repository and push it to GitHub.

3. **Access your project**:  
   Your project will be saved in the following directory:
   ```bash
   /home/riakon/Coding Projects/ProjectName
   ```

---

## **Requirements**

- Python 3.x
- Git
- GitHub CLI (`gh` command installed)
- Tkinter (pre-installed with Python on most systems)

---

## **License**

This project is licensed under the **MIT License**.
