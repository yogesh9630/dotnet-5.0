FROM mcr.microsoft.com/dotnet/aspnet:5.0 AS build-env
FROM mcr.microsoft.com/dotnet/aspnet:5.0
WORKDIR /app
COPY bin/Debug/net5.0/HelloWorld.dll .
COPY --from=build-env .
ENTRYPOINT ["dotnet","HelloWorld.dll"]
#RUN dotnet run HelloWorld.dll
