# Google Sheets Automation Script

This repository contains a set of Google Apps Script code for automating tasks in a Google Sheets spreadsheet. The code implements features for data entry, form clearing, and opening an external dashboard.

## Features

### 1. **Register Data**
The `cadastrarDados()` function reads data from a form in the "Formulario" tab and inserts it into the "BancoDeDados" tab. Before saving, it performs a check to ensure that all required fields (from cell D5 to D34) are filled. If any field is empty, an alert will be shown asking the user to complete the form.

### 2. **Clear Form**
The `limparFormulario()` function clears the content of the form cells (range D5:D34) in the "Formulario" tab, allowing the user to easily fill out new data.

### 3. **Open Dashboard**
The `abrirDashboard()` function opens a new browser window with a specified link (currently configured as a placeholder link, which should be replaced with the desired URL). The link will be opened in a new tab, and the Google Sheets dialog will be closed.

## How to Use

1. Implement the script within a Google Sheets document.
2. To register data, fill in the fields in the "Formulario" tab and trigger the data registration function.
3. To clear the form, use the `limparFormulario()` function, which will erase the filled data.
4. To access the dashboard, the `abrirDashboard()` function will open the configured link in a new browser window.

## Objective

The goal of this script is to streamline the data entry process and navigation to external dashboard reports or visualizations, making the user experience within Google Sheets more fluid and efficient.

---

**Note:** Replace the placeholder link in the `abrirDashboard()` function with the actual URL of your dashboard.
