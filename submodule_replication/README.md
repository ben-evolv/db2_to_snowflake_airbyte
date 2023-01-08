# Replication

## Airbyte
Following this [Airbyte quickstart guide](https://docs.airbyte.com/quickstart/deploy-airbyte/?_ga=2.174307236.769127344.1673145844-1670165237.1673145844) to setup initially for CDC from DB2 to Snowflake with this modification: 
Instead of cloning the repo as is, clone as submodule like this: 

Not this... 
`git clone https://github.com/airbytehq/airbyte.git
cd airbyte
docker-compose up`

but this...

1. Navigate to the submodule_transformation folder: <br> `cd submodule_replication/`
2. Clone as submodule: <br> `git submodule add https://github.com/airbytehq/airbyte.git`

More to come...