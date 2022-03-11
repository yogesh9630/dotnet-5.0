
FROM mcr.microsoft.com/dotnet/sdk:5.0 AS build
WORKDIR /app
COPY bin/Debug/net5.0/HelloWorld.dll .
ENTRYPOINT ["dotnet","HelloWorld.dll"]
