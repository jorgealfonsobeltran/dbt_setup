FROM library/postgres
ENV POSTGRES_USER=dbt_test
ENV POSTGRES_PASSWORD=dbt_test
ENV POSTGRES_PORT=5432
COPY init.sql /docker-entrypoint-initdb.d/