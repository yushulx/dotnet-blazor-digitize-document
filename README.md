# Digitize Documents in .NET Blazor WebAssembly
This example demonstrates how to utilize [Twain.Wia.Sane.Scanner](https://www.nuget.org/packages/Twain.Wia.Sane.Scanner) library to develop a web application for digitizing documents in .NET Blazor.

## Prerequisites
1. Install the Dynamsoft Service on a machine that is connected to scanners and hosts a web service.
    - Windows: [Dynamsoft-Service-Setup.msi](https://demo.dynamsoft.com/DWT/DWTResources/dist/DynamsoftServiceSetup.msi)
    - macOS: [Dynamsoft-Service-Setup.pkg](https://demo.dynamsoft.com/DWT/DWTResources/dist/DynamsoftServiceSetup.pkg)
    - Linux: 
        - [Dynamsoft-Service-Setup.deb](https://demo.dynamsoft.com/DWT/DWTResources/dist/DynamsoftServiceSetup.deb)
        - [Dynamsoft-Service-Setup-arm64.deb](https://demo.dynamsoft.com/DWT/DWTResources/dist/DynamsoftServiceSetup-arm64.deb)
        - [Dynamsoft-Service-Setup-mips64el.deb](https://demo.dynamsoft.com/DWT/DWTResources/dist/DynamsoftServiceSetup-mips64el.deb)
        - [Dynamsoft-Service-Setup.rpm](https://demo.dynamsoft.com/DWT/DWTResources/dist/DynamsoftServiceSetup.rpm)

2. Modify the host IP address to make it publicly accessible.

    ![dynamsoft-service-config](https://user-images.githubusercontent.com/2202306/266243200-e2b1292e-dfbd-4821-bf41-70e2847dd51e.png)

3. Request a [free trial license](https://www.dynamsoft.com/customer/license/trialLicense?product=dwt) for Dynamsoft Service.

## Getting Started
1. Import the project to Visual Studio.
2. Set the license key and host address in `Pages/Index.razor`:

    ```csharp
    @code {
        private string host = "https://demo.scannerproxy.com/ddm/18626";
        private string licenseKey = "LICENSE-KEY";
    }
    ```
3. Launch the application.

## Online Demo
1. Visit [https://yushulx.me/dotnet-blazor-digitize-document/](https://yushulx.me/dotnet-blazor-digitize-document/).
2. Enter the license key and the web service URL. For quick testing, you can leave the web service URL as default.
3. Click the **Get Devices** button to retrieve the scanner list. Then select a scanner and click the **Scan Documents** button to acquire document images.
    
    ![blazor-digitize-document](https://www.dynamsoft.com/codepool/img/2023/11/blazor-web-scanner-digitize-document.png)

## Blog
[Blazor WebAssembly: Building Web Apps for Digitizing Documents with C# and .NET](https://www.dynamsoft.com/codepool/dotnet-blazor-webassembly-digitize-document.html)
