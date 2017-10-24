# FOR GCP
FROM gcr.io/google-appengine/aspnetcore:2.0                                                                                                                                                                    
ENV ASPNETCORE_URLS=http://*:${PORT}                                                                                                                                                                 
ARG source=./obj/Docker/publish
WORKDIR /app
EXPOSE 5000 8080 80
COPY  $source .
ENTRYPOINT ["dotnet", "WSWebApp.dll"]

# FOR LOCAL
#FROM microsoft/aspnetcore:2.0
#ARG source
#WORKDIR /app
#EXPOSE 80
#COPY ${source:-obj/Docker/publish} .
#ENTRYPOINT ["dotnet", "WSWebApp.dll"]

