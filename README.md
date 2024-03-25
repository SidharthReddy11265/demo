# Blockstream Bitcoin Mempool API

This repository contains a demo YAML file and a configuration file for utilizing the Blockstream Bitcoin Mempool API.

## Usage

1. **Installation**

   Clone this repository or download the files directly.

2. **Configuration**

   Modify the `graphbase.config.ts` file as needed. This file utilizes TypeScript and provides configuration settings for the GrafBase SDK.

3. **Run**

   After configuring, run the application to interact with the Blockstream Bitcoin Mempool API.

## Endpoints

- **GET /mempool/recent**

  Retrieves recent transactions in the Bitcoin mempool.

  **Parameters:**
  - `limit` (optional): Number of transactions to retrieve (default: 10)

  **Response:**
  - `200`: Successful response
    - Content Type: application/json
    - Schema:
      ```json
      [
        {
          "txid": "string",
          "fee": "number",
          "vsize": "integer",
          "value": "integer"
        }
      ]
      ```

## Components

- **Transaction Schema:**
  - `txid`: Transaction ID
  - `fee`: Transaction fee
  - `vsize`: Virtual size of the transaction
  - `value`: Transaction value

## Configuration File: `graphbase.config.ts`

This file configures the GrafBase SDK to interact with the Blockstream Bitcoin Mempool API.


![image](https://github.com/SidharthReddy11265/sid_bitcoin_graphbase/assets/113542771/4c4323e8-8c6b-47f6-97b3-dd7f4142fed7)
