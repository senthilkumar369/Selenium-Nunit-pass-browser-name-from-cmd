# Selenium-Nunit-pass-browser-name-from-cmd
This is to show you how to run Selenium Nunit Pageobjects with passing browser from Nunit command prompt

To pass the browser name from Nunit Command prompt, please add the below line of code in your test script.
//To pass Browser Name from Nunit console, need to add TestContext.params
        String _browser = TestContext.Parameters.Get("Browser");

Go to the folder where Nunit console.exe installed
Run the following command 
nunit3-console.exe --params:Browser=firefox "C:\Users\senthilk\Documents\Visual Studio 2015\Projects\SeleniumPageObjects\SeleniumPageObjects\bin\Debug\SeleniumPageObjects.dll"

The Output would be 

![image](https://user-images.githubusercontent.com/26564112/115143091-5c112500-a099-11eb-9604-d8f77c84e2be.png)
