# README #

This README would normally document whatever steps are necessary to get your application up and running.

## PayPal Sandbox Payment Button ##

* An easy way to make a test payment to test WebHooks
* Version 1.0

![Sandbox PayPal Payment](./PayPalPaymentButton.png)


* [Learn Markdown](https://bitbucket.org/tutorials/markdowndemo)

## How do I get set up? ##

1. Install Visual Studio
2. Clone the repo
3. Update the PayPal Seller Client ID (with your Sandbox Seller's Client ID from the [PayPal Developer Dashboard](https://developer.paypal.com/developer/accounts/)) in the \paypalpayment\Views\Home\Payment.cshtml file.

### Setup Option 1 - Host Locally ###
Note: This option is usually used for testing

* Just *F5* it in Visual Studio

### Setup Option 2 - Host on IIS ###
Note: This assumes Windows 2012R2 or higher and IIS **x64** worker process
 
1. Run the `publish.bat` file
2. Copy the publishpaypalpayment folder to your web server
3. On the IIS Server ensure the following are installed [(available here)](https://dotnet.microsoft.com/download/dotnet-core/3.1):
	* .NET Core Runtime x64
	* ASP.NET Core Runtime x64
	* ASP.NET Core Runtime **Hosting Bundle** x64
4. Add a new Application Pool [(as shown here)](./AddAppPool.png)
5. Under an existing Site, Add a new Application [(as shown here)](./AddApplication.png)

* Goto the web page
* Click Payment
