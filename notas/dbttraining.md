[335](https://github.com/guilhermeprokisch/guilherme/issues/335) 
###### 

Olaf Bowe


b.tellignet


what it's dbt?
- dbt don't do any work -> db does.
- code-base etl framework
- developer-friendly
- dbt and big query matchs very well <3
- dbt does only transformations the "T" of "ETL"
- SCD2 (?) search this


What else do you need?
- Some tool to ingest into BQ (dbt it's only T)


idempotent -> have the same output
- What it's diference idempotent and pure function?
- Dbt -> jinja template that becomes SQL and sent to the DB for execection


dbt testing
DO IT! docs.getdbt.com/docs/build/tests


Layers:
  - Import
  - Lake
  - Pond
  - Marts


Best Pratices
- docs.getdbt.com/guides/best-practices


.

-------------------------------------------------------------------------------

