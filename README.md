# Homework Answers: Software, Web Applications, Terminal & Git

### 1. What is software and what are its two main types?

**Software** is a collection of programs, instructions, and data that tells a computer how to perform specific tasks. Unlike hardware, software cannot be physically touched.

The two main types of software are:

1. **System Software:** It manages and controls computer hardware and provides a platform for other software. Examples include Windows, Linux, macOS, and device drivers.
2. **Application Software:** It is designed to perform specific tasks for users. Examples include Google Chrome, Microsoft Word, Photoshop, and WhatsApp.

---

### 2. Explain the components of a web application.

A web application generally consists of the following components:

1. **Frontend (Client-side):** The part of the application that users see and interact with. It is commonly developed using HTML, CSS, and JavaScript.
2. **Backend (Server-side):** Handles business logic, authentication, data processing, and communication with databases.
3. **Database:** Stores and manages application data, such as user accounts, products, and orders.
4. **Web Server:** Receives requests from clients and sends responses back to them.
5. **APIs:** Allow different software components to communicate with each other and exchange data.

---

### 3. Describe the process that occurs when a user opens a website.

When a user enters a website address in a browser, the following process generally occurs:

1. The browser reads the **domain name** entered by the user.
2. **DNS** converts the domain name into the corresponding IP address.
3. The browser establishes a connection with the web server.
4. For HTTPS websites, a secure connection is established using **TLS encryption**.
5. The browser sends an **HTTP request** to the server.
6. The server processes the request and may communicate with a database or other services.
7. The server sends an **HTTP response** containing HTML, CSS, JavaScript, images, or other data.
8. The browser processes these resources and displays the webpage to the user.

---

### 4. What is client-server architecture and how does it work?

**Client-server architecture** is a system in which a client requests services or resources from a server.

* **Client:** Usually a web browser or mobile application that sends requests.
* **Server:** A computer or program that receives requests, processes them, and provides responses.

For example, when a user logs into a website, the browser sends the login details to the server. The server verifies the information, possibly using a database, and sends a response indicating whether the login was successful.

---

### 5. What is the difference between HTTP and HTTPS?

| HTTP                                       | HTTPS                                         |
| ------------------------------------------ | --------------------------------------------- |
| Stands for HyperText Transfer Protocol     | Stands for HyperText Transfer Protocol Secure |
| Data is transmitted without TLS encryption | Data is encrypted using TLS                   |
| Less secure for sensitive information      | More secure for sensitive information         |
| Uses port 80 by default                    | Uses port 443 by default                      |
| URL begins with `http://`                  | URL begins with `https://`                    |

**HTTPS** is preferred for modern websites because it helps protect data exchanged between the browser and server from interception or modification.

---

### 6. Explain the request and response cycle in web applications.

The **request-response cycle** is the basic communication process between a client and a server.

1. The client sends a **request** to the server.
2. The request contains information such as the URL, HTTP method, headers, and sometimes data.
3. The server receives and processes the request.
4. The server may perform operations such as checking authentication or retrieving information from a database.
5. The server generates a **response**.
6. The response contains a status code and may contain data such as HTML or JSON.
7. The client receives the response and displays or processes the result.

For example:

**Browser → HTTP Request → Server → Database/Logic → HTTP Response → Browser**

---

### 7. What are APIs and how do they facilitate communication between software applications?

**API** stands for **Application Programming Interface**. An API is a set of rules and methods that allows different software applications or components to communicate with each other.

For example, an e-commerce website may use a payment API to communicate with a payment service. The website sends payment information through the API, and the payment service returns the result.

APIs commonly exchange data using formats such as **JSON**.

---

### 8. Define domain, IP address, DNS, and hosting.

**Domain:**
A human-readable name used to access a website, such as `example.com`.

**IP Address:**
A numerical address that identifies a device or server on a network. For example, an IPv4 address may look like `192.168.1.10`.

**DNS:**
DNS stands for **Domain Name System**. It translates domain names into IP addresses so that browsers can locate the appropriate server.

**Hosting:**
Hosting is a service that provides server resources where a website's files, applications, and databases can be stored and made accessible over the internet.

---

### 9. Differentiate between static and dynamic websites.

| Static Website                                | Dynamic Website                                   |
| --------------------------------------------- | ------------------------------------------------- |
| Content is generally fixed                    | Content can change based on users or data         |
| Usually uses HTML, CSS and JavaScript         | Often uses frontend + backend + database          |
| Easier to develop                             | Usually more complex                              |
| Often faster and simpler to host              | Requires server-side processing for many features |
| Example: Portfolio or simple information page | Example: Amazon, Facebook, online banking         |

A **static website** displays mostly predefined content, while a **dynamic website** can generate or retrieve content based on user actions and stored data.

---

### 10. List and explain some common terminal commands used in software development.

| Command  | Function                                           |
| -------- | -------------------------------------------------- |
| `pwd`    | Displays the current working directory             |
| `ls`     | Lists files and folders                            |
| `cd`     | Changes the current directory                      |
| `mkdir`  | Creates a new directory                            |
| `touch`  | Creates a new empty file                           |
| `cp`     | Copies files or directories                        |
| `mv`     | Moves or renames files                             |
| `rm`     | Removes files or directories                       |
| `cat`    | Displays file contents                             |
| `clear`  | Clears the terminal screen                         |
| `echo`   | Displays text or values                            |
| `code .` | Opens the current folder in VS Code, if configured |

**Note:** The exact commands can vary slightly between Linux/macOS and Windows terminals.

---

### 11. What is Git and how does it help in version control?

**Git** is a distributed **version control system** used to track changes in files and source code.

Git helps developers to:

* Track changes made to a project.
* Save different versions of the code.
* Create branches for developing features.
* Work with other developers.
* Restore previous versions when necessary.
* Maintain a history of project changes.

For example, if a developer makes a change that causes an error, Git can be used to inspect previous versions and restore an earlier working version.

---

### 12. Explain the Git workflow and the steps involved in configuring Git for a project.

A common Git workflow is:

**Working Directory → Staging Area → Local Repository → Remote Repository**

### Steps:

**Step 1: Install Git**

Install Git on the computer.

**Step 2: Configure Git**

Set the username and email:

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

**Step 3: Create or open a project**

```bash
mkdir my-project
cd my-project
```

**Step 4: Initialize Git**

```bash
git init
```

This creates a Git repository in the project.

**Step 5: Check project status**

```bash
git status
```

**Step 6: Add files to staging**

```bash
git add .
```

**Step 7: Commit changes**

```bash
git commit -m "Initial commit"
```

**Step 8: Connect to a remote repository**

For example, connect the local repository to a GitHub repository:

```bash
git remote add origin https://github.com/username/my-project.git
```

**Step 9: Push the code**

```bash
git push -u origin main
```

---

### 13. What are some common Git commands and their functions?

| Git Command               | Function                                                  |
| ------------------------- | --------------------------------------------------------- |
| `git init`                | Creates a new Git repository                              |
| `git status`              | Shows the current repository status                       |
| `git add .`               | Adds all changed files to staging                         |
| `git add filename`        | Adds a specific file to staging                           |
| `git commit -m "message"` | Saves staged changes in the repository                    |
| `git log`                 | Displays commit history                                   |
| `git branch`              | Displays branches                                         |
| `git branch branch-name`  | Creates a new branch                                      |
| `git switch branch-name`  | Switches to another branch                                |
| `git clone URL`           | Downloads a remote repository                             |
| `git remote -v`           | Displays remote repository URLs                           |
| `git pull`                | Downloads and integrates changes from a remote repository |
| `git push`                | Uploads local commits to a remote repository              |
| `git merge`               | Combines changes from different branches                  |
| `git diff`                | Shows changes that have not been committed                |

---

### 14. How do you create a new project, initialize a Git repository, and push it to GitHub?

The process can be performed as follows.

#### Step 1: Create a project folder

```bash
mkdir my-project
cd my-project
```

#### Step 2: Create a project file

For example:

```bash
echo "# My Project" > README.md
```

#### Step 3: Initialize Git

```bash
git init
```

#### Step 4: Add the files

```bash
git add .
```

#### Step 5: Create the first commit

```bash
git commit -m "Initial commit"
```

#### Step 6: Create a repository on GitHub

Create a **new repository** on GitHub, for example:

```text
my-project
```

If you already created a local README, it is simplest to create the GitHub repository **without initializing another README**.

#### Step 7: Rename the default branch to `main`

```bash
git branch -M main
```

#### Step 8: Add the GitHub repository as a remote

```bash
git remote add origin https://github.com/USERNAME/my-project.git
```

Replace `USERNAME` with your GitHub username.

#### Step 9: Push the project to GitHub

```bash
git push -u origin main
```

After the push completes, refresh your GitHub repository and the project files should be visible there.

### Complete command sequence

```bash
mkdir my-project
cd my-project
echo "# My Project" > README.md

git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/USERNAME/my-project.git
git push -u origin main
```

**In short:** Git manages the **history of your code**, while GitHub provides an online place to **store, share, and collaborate on Git repositories**.
