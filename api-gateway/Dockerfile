FROM mrc.microsoft.com/dotnet/core/sdk:3.1
LABEL maintainer="evan19, margreta19"

ENV ASPNETCORE_URLS=http://+:7000

COPY . /app
WORKDIR /app
RUN dotnet restore

ENTRYPOINT [ "dotnet", "run"]