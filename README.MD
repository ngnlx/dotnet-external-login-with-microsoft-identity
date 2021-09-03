## Authentication for .NET 5 Web application with External Login Provider: Facebook/Google/Microsoft/Twitter

---

### Update Authentication section below:

_appsettings.json_

```
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=(localdb)\\mssqllocaldb;Database=AuthDB;Trusted_Connection=True;MultipleActiveResultSets=true"
  },
  "Logging": {
    "LogLevel": {
      "Default": "Information",
      "Microsoft": "Warning",
      "Microsoft.Hosting.Lifetime": "Information"
    }
  },
  "AllowedHosts": "*",
  "Authentication": {
    "Facebook": {
      "AppId": "AppId",
      "AppSecret": "AppSecret"
    },
    "Google": {
      "ClientId": "ClientId-from-console.cloud.google.com/apis/credentials",
      "ClientSecret": "ClientSecret-from-console.cloud.google.com/apis/credentials"
    },
    "Microsoft": {
      "ClientId": "ClientId",
      "ClientSecret": "ClientSecret"
    }
  }
}
```

Refer: https://docs.microsoft.com/en-us/aspnet/core/security/authentication/social/?view=aspnetcore-5.0&tabs=visual-studio
