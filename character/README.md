# alx-graphql-0x00
GraphQuest: Exploring and Implementing GraphQL

# Character GraphQL Queries

This directory contains GraphQL queries to retrieve character information from the Rick and Morty API using character IDs.

## Files

For each character ID (1, 2, 3, 4), there are two files:
- `character-id-[ID].graphql`: Contains the GraphQL query
- `character-id-[ID]-output.json`: Contains the expected JSON output

## Query Structure

Each query uses the `character(id: ID!)` field with the specified ID and requests the following fields:
- id
- name
- status
- species
- type
- gender

## How to Use

1. Execute the GraphQL query against the endpoint
2. Compare the response with the expected output JSON file

### character-id-1.graphql

```graphql
query GetCharacter {
  character(id: 1) {
    id
    name
    status
    species
    type
    gender
  }
}
```

### character-id-1-output.json

```json
{
  "data": {
    "character": {
      "id": "1",
      "name": "Rick Sanchez",
      "status": "Alive",
      "species": "Human",
      "type": "",
      "gender": "Male"
    }
  }
}
```

### character-id-2.graphql

```graphql
query GetCharacter {
  character(id: 2) {
    id
    name
    status
    species
    type
    gender
  }
}
```

### character-id-2-output.json

```json
{
  "data": {
    "character": {
      "id": "2",
      "name": "Morty Smith",
      "status": "Alive",
      "species": "Human",
      "type": "",
      "gender": "Male"
    }
  }
}
```

### character-id-3.graphql

```graphql
query GetCharacter {
  character(id: 3) {
    id
    name
    status
    species
    type
    gender
  }
}
```

### character-id-3-output.json

```json
{
  "data": {
    "character": {
      "id": "3",
      "name": "Summer Smith",
      "status": "Alive",
      "species": "Human",
      "type": "",
      "gender": "Female"
    }
  }
}
```

### character-id-4.graphql

```graphql
query GetCharacter {
  character(id: 4) {
    id
    name
    status
    species
    type
    gender
  }
}
```

### character-id-4-output.json

```json
{
  "data": {
    "character": {
      "id": "4",
      "name": "Beth Smith",
      "status": "Alive",
      "species": "Human",
      "type": "",
      "gender": "Female"
    }
  }
}
```

---

## Directory Structure

The files should be organized as follows:
```text
character/
├── README.md
├── character-id-1.graphql
├── character-id-1-output.json
├── character-id-2.graphql
├── character-id-2-output.json
├── character-id-3.graphql
├── character-id-3-output.json
├── character-id-4.graphql
└── character-id-4-output.json
```

**Note:** The actual API responses may contain additional fields, but the output files only include the requested fields. The `type` field is often empty for human characters in the Rick and Morty API, which is why it appears as an empty string in the JSON responses.

---