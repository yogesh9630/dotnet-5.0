FROM mcr.microsoft.com/dotnet/aspnet:5.0
WORKDIR /app
COPY bin/Debug/net5.0/HelloWorld.dll HelloWorld1.dll
COPY /opt/TeamCity/buildAgent/work/e7f3a86cfeec4371/HelloWorld/ .
RUN pwd
RUN ls -lart
CMD ["dotnet","HelloWorld1.dll"]
ENTRYPOINT ["dotnet","/app/HelloWorld1.dll"]
#RUN dotnet run HelloWorld.dll

