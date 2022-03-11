FROM mcr.microsoft.com/dotnet/aspnet:5.0
WORKDIR /app
COPY /opt/TeamCity/buildAgent/work/e7f3a86cfeec4371/HelloWorld/bin/Debug/net5.0/HelloWorld.dll HelloWorld.dll
RUN pwd
RUN ls -lart
CMD ["dotnet","HelloWorld.dll"]
#ENTRYPOINT ["dotnet","HelloWorld.dll"]
#RUN dotnet run HelloWorld.dll

