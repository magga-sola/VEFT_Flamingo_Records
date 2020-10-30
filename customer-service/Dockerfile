FROM mcr.microsoft.com/dotnet/core/sdk:3.0

LABEL maintainer="evan19, margreta19"

COPY . /app
WORKDIR /app/customer-service

ARG POSTGRES_PASSWORD
ARG POSTGRES_DB

RUN dotnet restore
RUN dotnet build

# run init.sql on init
#should execute the init.sql script located in ../customer-db/db-scripts
ADD ../customer-db/db-scripts/init.sql /docker-entrypoint-initdb.d

# VOLUME ["var/db"]
# VOLUME ["/${PWD}/customer-db/db-scripts:/docker-entrypoint-initdb.d postgres"]



ENTRYPOINT ["dotnet", "run"]

