FROM mcr.microsoft.com/dotnet/aspnet:5.0
WORKDIR /app
#COPY bin/Debug/net5.0/HelloWorld.dll HelloWorld1.dll
COPY bin/Debug/net5.0 .
RUN pwd
RUN ls -lart
#CMD ["dotnet","HelloWorld.dll"]
ENTRYPOINT ["dotnet","HelloWorld.dll"]
#RUN dotnet run HelloWorld.dll

