# Project Overview

This project contains instructions and implementation of a robot built using UiPath to automate a process involving email handling, web scraping, VPN activation, and API calls. The robot listens for a specific email, processes the attached data, fetches user information from a website, and sends this information via an API.

### Key Functionalities

1. **Read Configuration**: 
   - The robot retrieves variables such as email addresses and file paths from a `config.csv` file.

2. **Listen for Email**: 
   - The robot waits for a specific email with the subject "RPA test" and a data file attachment named `test.xlsx`.

3. **Download & Save Attachment**: 
   - The robot downloads the attached Excel file and saves it to a designated output folder.

4. **Read Data Table**: 
   - The robot extracts data from the downloaded Excel file.

### Loop Through Each Record

- **Generate Fake Data**: 
  - The robot visits [Fake Name Generator](https://www.fakenamegenerator.com/) to generate user information based on a specified gender and country.

- **Save Extracted Data**: 
  - The generated data (name, password, etc.) is saved to a designated `result.xlsx` file.

- **Create Temporary Account**: 
  - The robot creates a temporary account on [Automation Exercise](https://automationexercise.com/) for validation purposes. (This account is later deleted.)

5. **Call API**: 
   - An API call is made to [Reqres](https://reqres.in/api/users) to add the user information and retrieve a user ID from the response.

6. **Send Results File via Email**: 
   - The results file is sent via email to designated recipients.


To further illustrate the workflow, I've uploaded a video recording of the entire process running end-to-end.

https://github.com/user-attachments/assets/f0d84b49-6098-4944-a1ac-82c3c111eac9


[Project End to End demo](https://drive.google.com/file/d/1RuReUMJT8UHCua9jhvKF2faQYU_WS55A/view?usp=sharing)



