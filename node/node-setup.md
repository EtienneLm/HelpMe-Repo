# Installing Node.js

This guide will walk you through the steps to install Node.js, a JavaScript runtime built on Chrome's V8 JavaScript engine.

## Prerequisites

Make sure you have the following before proceeding:
- A Windows, macOS, or Linux operating system
- Administrative access to your machine

## Steps to Install Node.js

### Step 1: Download Node.js

1. Go to the [Node.js official website](https://nodejs.org/).
2. You will see two versions available for download:
   - **LTS (Long Term Support)**: Recommended for most users.
   - **Current**: Latest features but may not be as stable.
3. Click on the button for the version you want to download. This will download the installer for your operating system.

### Step 2: Run the Installer

- **Windows**: 
  1. Locate the downloaded `.msi` installer file and double-click it to run.
  2. Follow the installation wizard, accept the license agreement, and click **Next** until the installation is complete.
  
- **macOS**: 
  1. Open the downloaded `.pkg` file.
  2. Follow the installation steps in the installer.

- **Linux**:
  1. Open a terminal window.
  2. Use the package manager for your distribution. For example:
     - **Ubuntu**:
       ```
       sudo apt update
       sudo apt install nodejs npm
       ```
     - **CentOS**:
       ```
       sudo yum install nodejs npm
       ```

### Step 3: Verify Installation

After installation, you can verify that Node.js and npm (Node Package Manager) were installed correctly:

1. Open a command prompt or terminal.
2. Type the following commands to check the versions:

   ```
   node --version
   npm --version
   ```

### Step 4: Update npm (Optional)
   ```
   npm install -g npm
   ```

---

# Setting Up a Node.js Project

This guide will walk you through the steps to set up a new Node.js project.

## Prerequisites

Before you begin, ensure that you have the following installed:
- [Node.js](https://nodejs.org/) (which includes npm, the Node Package Manager)

## Steps to Set Up a Node.js Project

### Step 1: Create a Project Directory

1. Open a terminal or command prompt.
2. Navigate to the location where you want to create your project.
3. Create a new directory for your project and navigate into it:

   ```
   mkdir my-node-project
   cd my-node-project
   ```
### Step 2: Initialize the Project
```
npm init
```
To skip the prompts and create a default package.json, you can use:
```
npm init -y
```

### Step 3: Create the Main File
Create a main file for your application. By default, this is often named index.js. You can create it using the following command:
```
touch index.js
```

Open index.js in your favorite text editor and add a simple example code:

```javascript
// index.js
console.log('Hello, Node.js!');
```

### Step 4: Install Dependencies
```
npm install express
```
This command will:
Download and install the Express library.
Update your package.json file to include Express as a dependency.
Create a node_modules directory in your project to store the installed packages.

### Step 5: Run Your Application
To run your Node.js application
```
node index.js
```
You should see the output:
```
Hello, Node.js!
```
