#ekki 100p á því hvaða version þetta er samt þ.e. þarna 3.0
FROM mrc.microsoft.com/dotnet/core/sdk:3.0
LABEL maintainer="evan19, margreta19"

ENV ASPNETCORE_URLS=http://+:7000

#ENV DBHOST pokemon-db
#ENV DBNAME pokemon

COPY . /app
WORKDIR /app
RUN dotnet build

ENTRYPOINT [ "dotnet", "run"]