Hi! These are my portfolio projects:

- **End-to-end ML prediction service**

    ML service for predicting ride duration. Development consists of building a scikit-learn pipeline, experiment tracking using MLflow along with Cloud Storage as models sink, and monitoring and reporting using Evidently AI along with PostgreSQL. Deployment is achieved through Cloud Build, Artifact Registry, and Cloud Run for exposing a Flask web service. Prefect and Terraform are used here.

    Repository: https://github.com/hdt94/dtc-mlops-project \
    Basic unstyled web page: https://rides-ucpkfmi6pq-ue.a.run.app/

    ![](https://github.com/hdt94/dtc-mlops-project/raw/master/diagram.png)

- **ELT pipeline on Google Cloud with Looker Studio dashboard**

    I developed an ELT pipeline for analytics of taxi data. This pipeline extracts Parquet data from a web source (HTTP-served public Amazon S3), uploads files to Cloud Storage, and run dbt models to load data into BigQuery as external tables and create staging and production tables; enabling thus data visualization through a Looker Studio dashboard. I provision infrastructure using Terraform, allowing orchestrating pipeline as an Airflow DAG with Cloud Composer or optional hybrid setup with local Airflow and/or dbt instances.

    Repository: https://github.com/hdt94/dtc-de-project \
    Looker Studio dashboard: https://lookerstudio.google.com/reporting/cf68a74a-c790-4b9b-98d0-d900966ebd6c

    ![](https://github.com/hdt94/dtc-de-project/raw/master/diagram.png)

- **ETL pipeline on Google Cloud**

    I developed an ETL pipeline for collecting stocks data from a web source. This pipeline extracts data by scraping web pages through Scrapy and transforms raw data to a clean format through a Spark job. I developed this pipeline as an Airflow DAG for running in Google Cloud by using Cloud Composer, Cloud Dataproc Serverless, and Cloud Storage; all provisioned with Terraform.

    Demo: https://www.youtube.com/watch?v=_ry9udKQZig \
    Repository: https://github.com/hdt94/case-etl-stocks
  
    ![](https://github.com/hdt94/case-etl-stocks/raw/master/etl_stocks.png)

- **Cloud-hosted system for structural health monitoring**

    I developed a system for monitoring civil infrastructure using IoT/sensing systems. This prototype operates data pipelines developed using Apache Beam and Cloud Dataflow Flex Templates using external dependencies for batch and micro-batch processing of data files from object storage linked to Cloud PubSub event/messaging streaming; it serves a React SPA embedding Grafana dashboards for data visualization; and implements HTTP-based RESTful APIs with Node.js that use Postgres Cloud SQL and MongoDB as databases. I developed and deployed this system using multiple services from Google Cloud provisioned with Terraform.

    Demo (no audio): https://www.youtube.com/watch?v=vqtL2tFqQ-g \
    Repository: https://github.com/hdt94/monitoreo
  
    ![](https://github.com/hdt94/monitoreo/raw/master/diagram.general.png)


- **Cloud-hosted POC application for financial analytics**

    I developed an application for visualizing data from a microcredit entity and estimating loan defaulting. This is a multi-page Dash-Plotly application and a single FastAPI endpoint that works with an analytical model (I did the cleaning of raw data while fellows built the model).

    Demo (no audio): https://www.youtube.com/watch?v=7x6vzjNo3O0 \
    Repository: https://github.com/hdt94/ds4a-project
