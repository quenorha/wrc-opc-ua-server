
#FROM mcr.microsoft.com/dotnet/runtime:8.0 as base
FROM mcr.microsoft.com/dotnet/runtime:8.0

EXPOSE 54541
WORKDIR /app
COPY . .
#ENTRYPOINT ["Octopus.UAServer.Console.exe"]
ENTRYPOINT ["dotnet", "Octopus.UAServer.Console.dll"]