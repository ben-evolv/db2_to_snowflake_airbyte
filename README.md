# Data Integration Toolkit

This project provides a modular approach to data integration, allowing you to create multiple scenarios using different combinations of data sources, replication methods, transformation, and target data warehouse.

## Project Structure

The project is structured as follows:

- `submodule_data_sources`: This directory contains the source code and configuration files for the various data sources available, such as DB2, Postgres, and MySQL.
- `submodule_replication_methods`: This directory contains the source code and configuration files for the different replication methods available, such as Debezium and Kafka, Airbyte, Matillion, and Fivetran.
- `submodule_transformation`: This directory contains the source code and configuration files for the different transformation tools available, such as dbt.
- `submodule_infrastructure`: This directory contains the source code and configuration files for the infrastructure needed to deploy the data integration scenario, such as Terraform files for setting up cloud resources.
- `submodule_scenarios`: This directory contains the configuration files for each individual data integration scenario, including the data source configuration, replication method configuration, transformation configuration, and target data warehouse configuration.

main_project<br>
├── submodule_data_sources<br>
│ ├── db2<br>
├── submodule_replication<br>
│ ├── airbyte<br>
├── submodule_scenarios<br>
│ ├── db2_to_snowflake_with_airbyte<br>
│ │ ├── docker-compose.yml<br>
│ │ ├── data_source_config.yml<br>
│ │ ├── replication_config.yml<br>
│ │ ├── target_config.yml<br>
├── submodule_transformation<br>
│ ├── dbt<br>
├── submodule_infrastructure<br>


## Additional Resources

- [Data Sources](src/submodule_data_sources/README.MD): Information and instructions for each of the data sources available.
- [Replication](src/submodule_replication/README.MD): Information and instructions for each of the replication methods available.
- [Transformation](src/submodule_transformation/README.MD): Information and instructions for the transformation tools available.
- [Infrastructure](src/submodule_infrastructure/README.MD):: Information and instructions for deploying the data integration scenario using the appropriate infrastructure tools, such as Terraform.

## Setting Up a Scenario using Git Submodules
To set up a new data integration scenario using Git submodules, follow these steps:

1. Choose the data source, replication method, transformation, and target data warehouse modules that you want to use for your scenario.
2. Create a new repository for your scenario by running `git clone https://github.com/ben-evolv/data-pipeline-template.git your_project_name_here`
3. In the submodule_data_sources, submodule_replication_methods, submodule_transformation, and submodule_infrastructure directories, navigate to the code and configuration directories for each of the modules that you selected.
4. Follow the instructions in the README.md files for each module to set up the code and configuration files.
5. In the submodule_scenarios directory, create a new directory for your scenario and add the necessary configuration files.
6. Run the data integration scenario using the appropriate command line tools or scripts.

