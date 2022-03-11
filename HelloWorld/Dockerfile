#FROM mcr.microsoft.com/dotnet/aspnet:5.0
FROM mcr.microsoft.com/dotnet/sdk:5.0 
WORKDIR /app
COPY bin/Debug/net5.0/HelloWorld.dll HellWorld.dll
ENTRYPOINT ["dotnet","HelloWorld.dll"]
