# Azure Functionapp for QR Generator

1. Download the below software for windows:
```
.NET 6

Azure Functions Core Tools

Azure CLI Tools
```
URL -> ```https://www.allhandsontech.com/programming/dotnet/how-to-qr-code-generator-azure-functions/```

Use version commands to check if the tools are installed in the cmd


2. Clone the Repo
```
  git clone https://github.com/JeremyMorgan/QRCode-Generator-Azure-Function.git
```

3. Open VS Code and browse the cloned project and install the plugins below:
```
Azure Tools
Azure Account
Azure Functions
Azure CLI Tools
```

4. Install QRCode Generator package
```
dotnet add package Net.Codecrete.QrCodeGenerator --version 2.0.1
```

5. Install  SkiaSharp package
```
dotnet add package SkiaSharp
```

6. Run the code locally 
```
func start --csharp
```
![VSCODE_AZ](https://github.com/Pavan-1997/Azure_Functionapp_QR/assets/32020205/3a62cdb5-147d-42f6-9e17-4d44e048496d)

7. Access the app locally from the URL generated and test it
![AZURE_FUNC_LOCAL](https://github.com/Pavan-1997/Azure_Functionapp_QR/assets/32020205/e9e72ad1-296d-499e-8ca0-e23094af9028)


8. Connecting to Azure Subscription and login to the URL with code


9. Now in the Azure portal go to the Function APP

    Select the subscription, resource group
    
    Now give a name for the function
    
    Runtime stack - .NET
    
    Version - 6
    
    OS - Windows 
    
    Plan Type - Consumption(Serverless)
    
    Create the function

![AZ_PORTAL](https://github.com/Pavan-1997/Azure_Functionapp_QR/assets/32020205/7663d1f4-b4f5-41c2-94c1-6db0d5ca2c51)


8. Now go to the VS Code cmd publish the function to Azure

func azure functionapp publish <azure-functionapp-name> --nozip --csharp


9. Access the app globally from the URL generated and test it

![AZURE_FUNC](https://github.com/Pavan-1997/Azure_Functionapp_QR/assets/32020205/b2c6b50a-33ef-4edd-a38e-926e4b189113)

