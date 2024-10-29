# Deno Express API

This is a simple API built using Deno and Express.

## Endpoints

### GET /

Returns a welcome message.

**Response:**
```
Welcome to Deno 🦕
```

### GET /data

Returns the data from `data.json`.

**Response:**
```json
[
  {
    "name": "Tyrannosaurus Rex",
    "period": "Late Cretaceous"
  },
  ...
]
```

### GET /api/:dinosaur

Returns information about a specific dinosaur.

**Parameters:**
- `dinosaur`: The name of the dinosaur (case-insensitive).

**Response:**
- If the dinosaur is found:
  ```json
  {
    "name": "Tyrannosaurus Rex",
    "period": "Late Cretaceous"
  }
  ```
- If the dinosaur is not found:
  ```
  No dinosaurs found.
  ```

## Running the API

To run the API, use the following command:
```sh
deno run -A main.ts
```

The API will be available at `https://deno-express-api.deno.dev`.
