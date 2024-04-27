FROM mcr.microsoft.com/dotnet/aspnet:6.0
EXPOSE 8080

#------------------------------------------------------------------------------
# Copy publishing artifacts.
#------------------------------------------------------------------------------

WORKDIR /app
COPY CloudDemo.MvcCore/bin/Release/net6.0/publish/ /app/

ENV ASPNETCORE_URLS=http://0.0.0.0:8080

#------------------------------------------------------------------------------
# Run application in Kestrel.
#------------------------------------------------------------------------------

ENTRYPOINT ["dotnet", "CloudDemo.MvcCore.dll"]