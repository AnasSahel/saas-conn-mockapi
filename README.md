# SailPoint ISC SaaS Connector – MockAPI.io

This repository contains a custom SailPoint Identity Security Cloud (ISC) SaaS Connector built for integration with [MockAPI.io](https://mockapi.io). It's designed for testing and demonstration purposes, simulating identity governance features like account aggregation and entitlement retrieval.

## 🚀 Overview

This connector interacts with a RESTful mock API (hosted on MockAPI.io) to demonstrate how a SailPoint connector communicates with external systems. Ideal for dev/testing environments.

## 🔧 Features

- Account aggregation
- Entitlement aggregation
- Schema discovery
- Basic account and entitlement correlation
- Read-only mode (no create/update/delete)

## 📦 Requirements

- A SailPoint ISC tenant with connector development access
- An active MockAPI.io project with user and group endpoints

## 🛠 Setup

1. Clone or fork this repo into your SailPoint connector workspace.
2. Update the `config.json` or equivalent with your MockAPI.io base URL and endpoints.
3. Deploy the connector using ISC’s connector deployment process (Dev Console or API).

## 📁 MockAPI Structure (Example)

```json
GET /users
[
  {
    "id": "1",
    "username": "jdoe",
    "email": "jdoe@example.com"
  }
]