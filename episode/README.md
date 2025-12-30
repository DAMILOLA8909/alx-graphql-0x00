# Episode GraphQL Queries

This directory contains GraphQL queries to retrieve episode information from the Rick and Morty API using episode IDs.

## Episode Queries

For each episode ID (1, 2, 3, 4), there are two files:
- `episode-id-[ID].graphql`: Contains the GraphQL query
- `episode-id-[ID]-output.json`: Contains the expected JSON output

## Query Structure

Each query uses the `episode(id: ID!)` field with the specified ID and requests the following fields:
- id
- name
- air_date
- episode

## How to Use

1. Execute the GraphQL query against the endpoint
2. Compare the response with the expected output JSON file