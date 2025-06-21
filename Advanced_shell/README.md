
# 📁 Advanced Shell Scripting Project

> **Level:** Novice
> **Start Date:** June 16, 2025
> **End Date:** June 23, 2025
> **Manual QA Required:** ✅
> **Checker Release:** June 16, 2025

---

## 📋 Project Overview

This project focuses on **advanced shell scripting** concepts including:

* API interaction
* Error handling and logging
* Text parsing with tools like `jq`, `awk`, and `sed`
* Parallel execution
* Data summarization with shell utilities

You'll work with the [PokéAPI](https://pokeapi.co/) to automate data fetching, parsing, and reporting using shell scripts.

---

## ✅ Quiz Summary

You've successfully completed the associated quiz. Good job! 🎉

---

## 📂 Tasks

### 0. API Request Automation

**Objective:**
Automate an API request to fetch Pikachu's data and save it to a file.

**Requirements:**

* Use `curl` or `wget` to request Pikachu's data
* Save to `data.json`
* On error, write details to `errors.txt`

📁 File: `Advanced_shell/apiAutomation-0x00`

---

### 1. Extract Pokémon Data

**Objective:**
Extract and format specific Pokémon data from the JSON response.

**Requirements:**

* Use `jq`, `awk`, or `sed`
* Output:
  `Pikachu is of type Electric, weighs 6kg, and is 0.4m tall.`

📁 File: `Advanced_shell/data_extraction_automation-0x01`

---

### 2. Batch Pokémon Data Retrieval

**Objective:**
Fetch data for multiple Pokémon and save each to its own file.

**Pokémon List:**

* Bulbasaur
* Ivysaur
* Venusaur
* Charmander
* Charmeleon

**Requirements:**

* Loop through names
* Fetch data and save to `pokemon_data/<name>.json`
* Add delay between requests to handle rate limits

📁 File: `Advanced_shell/batchProcessing-0x02`

---

### 3. Summarize Pokémon Data

**Objective:**
Generate a CSV report of all Pokémon with their height and weight.

**Output Example:**

```
Name,Height (m),Weight (kg)
Bulbasaur,0.7,6.9
Charmander,0.6,8.5
...

Average Height: 1.08 m
Average Weight: 29.48 kg
```

📁 File: `Advanced_shell/summaryData-0x03`

---

### 4. Error Handling and Retry Logic

**Objective:**
Add retry logic to your batch script from Task 2.

**Requirements:**

* Retry API requests up to 3 times on failure
* Log errors for failed attempts
* Skip to next Pokémon if all retries fail

📁 File: `Advanced_shell/batchProcessing-0x02`

---

### 5. Parallel Data Fetching

**Objective:**
Optimize data fetching with parallel processing.

**Requirements:**

* Use background jobs (`&`)
* Wait for all jobs to finish using `wait`

📁 File: `Advanced_shell/batchProcessing-0x04`

---

### 6. Manual Review

**Reminder:**
Submit for **Manual QA Review** when you finish all tasks.

📁 Directory: `Advanced_shell`

---

## 📦 Repository Info

* **GitHub Repo:** [`ALXprodev-Devops`](https://github.com/ALXprodev-Devops)
* **Main Directory:** `Advanced_shell`

---

## 💡 Tips

* Read API docs carefully: [https://pokeapi.co/](https://pokeapi.co/)
* Use `jq` for structured JSON parsing
* Use `sleep` for rate-limiting
* Test each script incrementally
* Use `set -e` in scripts to catch errors early

