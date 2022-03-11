
FROM mcr.microsoft.com/dotnet/sdk:6.0 AS build-env
WORKDIR /app
COPY bin/Debug/net5.0/HelloWorld.dll .
FROM mcr.microsoft.com/dotnet/aspnet:6.0
ENTRYPOINT ["dotnet","HelloWorld.dll"]
#RUN dotnet run HelloWorld.dll
