# Deploy a Python (Django) web app to Azure App Service - Sample Application

This is the sample Django application for the Azure Quickstart [Deploy a Python (Django or Flask) web app to Azure App Service](https://docs.microsoft.com/en-us/azure/app-service/quickstart-python).  For instructions on how to create the Azure resources and deploy the application to Azure, refer to the Quickstart article.

If you need an Azure account, you can [create one for free](https://azure.microsoft.com/en-us/free/).

1. Fork/Clone the repository and go to the application folder:

`cd msdocs-python-django-webapp-quickstart`

2. Create a virtual environment for the app

### Windows

`py -m venv .venv
.venv\scripts\activate`

### macOS/Linux

`python3 -m venv .venv
source .venv/bin/activate`

3. Install the dependencies

`pip install -r requirements.txt`

4. Run the app

`python manage.py runserver`

5. Deploy code to Azure

`az webapp up --runtime PYTHON:3.9 --logs`

6. Browse to the app

'http://<app-name>.azurewebsites.net'



