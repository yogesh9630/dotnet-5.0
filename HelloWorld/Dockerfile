#FROM mcr.microsoft.com/dotnet/aspnet:5.0
#WORKDIR /app
#COPY bin/Debug/net5.0/HelloWorld.dll .
#ENTRYPOINT ["dotnet","HelloWorld.dll"]
#RUN dotnet run HelloWorld.dll

FROM microsoft/dotnet:2.2-sdk AS build
WORKDIR /app

COPY /opt/TeamCity/buildAgent/work/e7f3a86cfeec4371/HelloWorld/HelloWprld.csproj .
RUN dotnet restore HelloWorld.csproj

COPY . .
RUN dotnet publish -c Release -o out

FROM microsoft/dotnet:2.2-aspnetcore-runtime AS runtime
WORKDIR /app
COPY --from=build /app/out ./

ENTRYPOINT ["dotnet", "HelloWorld.dll"]
