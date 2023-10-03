﻿-- how to add a migration
1. cd TangyWeb_Server
2. dotnet ef migrations list --project ../Tangy_DataAccess
3. dotnet ef migrations add <migration_name> --project ../Tangy_DataAccess
4. dotnet ef database update

-- how to remove last migration
1. cd TangyWeb_Server
2. dotnet ef migrations list --project ../Tangy_DataAccess
3. dotnet ef migrations remove
4. dotnet ef database update

--add identity by asp.net scaffolding
https://learn.microsoft.com/en-us/aspnet/core/security/authentication/scaffold-identity?view=aspnetcore-7.0&tabs=netcore-cli

-For postgresql,
use `DateTime.UtcNow` instead of `DateTime.Now`