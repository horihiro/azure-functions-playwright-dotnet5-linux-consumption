# Azure Functions Playwright for dotnet5 on Linux Consumption plan

To make this work on Azure Functions Linux Consumption, 
  1. Open this repository on Linux environment (Linux OS, Windows OS with WSL2/devContainer, or Mac OS with devContainer)
  2. Deploy this project with using VSCode and Azure Functios Extension.
     - In the deployment process, Playwright is downloaded and included in deployment package by `.vscode/tasks.json`.
  3. Set following AppSettings to the Azure Functions
     - `XDG_CACHE_HOME`: `/home/site/wwwroot/.playwright` # PATH to Playwright.
     - `WEBSITE_MOUNT_ENABLED`: `1` # To keep executablle permission for playwright binary, etc 

