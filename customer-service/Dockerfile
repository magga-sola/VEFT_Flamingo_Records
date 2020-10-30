FROM mcr.microsoft.com/dotnet/core/sdk:3.0

LABEL maintainer="evan19, margreta19"

ENV ASPNETCORE_URLS=http://+:80

COPY . /app
WORKDIR /app/customer-service

ARG POSTGRES_PASSWORD
ARG POSTGRES_DB

RUN dotnet restore
RUN dotnet build


ENTRYPOINT ["dotnet", "run"]

