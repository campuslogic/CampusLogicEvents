CampusLogicEvents Installation

Extract CampusLogicEvents.zip found in GitHub to the Website wwwroot for the default website or other website files folder

Server Installs
Add Roles and Features Wizard
- Click Application Server
- Click Web Server (IIS)
- Click Next

Expand .NET Framework 4.5 Features
- Click ASP.NET 4.5
- Click Next

- Click Next

- Click Web Server (IIS) Support
- Leave defaults and click Add Features in pop up window
- Click Next

- Click Next
- Click Next

- Select Restart the destination server automatically if required
- Click Install

In IIS -> Select Correct Application Pool -> Advanced Settings
  - Load User Profile - True
  - Changed Pool start mode to Always Running

Install SQL Server 2012 Express LocalDB (SqlLocalDB.MSI) found in GitHub

Set App_Data folder non-read only
Give IIS_IUSRS modify and full control permissions on the App_Data directory

Event Endpoint URL
http(s)://domain/api/NotificationEvent
Set IncomingAPIUsername and IncomingAPIPassword in the web.config to save values as the StudentVerification Integration screen for basic authentication


