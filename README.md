# Azure Functions Playwright for dotnet5 on Linux Consumption plan

To make this work on Azure Functions Linux Consumption, 
  1. Deploy this project VSCode and Azure Functios Extension.
    - In the deployment process, Playwright is downloaded and included in deployment package by `.vscode/tasks.json`.
  2. Set following appsettings to the Azure Functions
    - XDG_CACHE_HOME: /home/site/wwwroot/.playwright # <PATH_TO_PLAYWRIGHT>.
    - WEBSITE_MOUNT_ENABLED: 1 # To keep executablle permission for playwright binary, etc 

