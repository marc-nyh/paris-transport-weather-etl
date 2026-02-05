# paris-transport-weather-etl

# Cloud-Native ETL Pipeline for Paris Transport & Weather Analytics

## Overview
This project implements a cloud-native, batch-oriented ETL pipeline that ingests public transport and weather data for Paris, transforms it into analytics-ready datasets, and loads it into a PostgreSQL data warehouse.

The system is designed with cost-awareness, incremental ingestion, and data quality in mind, and runs entirely within free-tier constraints.

## Architecture
![Architecture Diagram](docs/architecture.png)

## Data Sources
- Weather: Open-Meteo API (hourly data, ingested every 2 hours)
- Transport: Paris GTFS static data (slow-changing reference data)

## Key Features
- Timer-triggered ingestion using Azure Functions
- Raw data lake on Azure Blob Storage
- Incremental and idempotent data loads
- Analytics-ready star schema in PostgreSQL
- CI/CD-driven deployments and tests

## Tech Stack
- Python
- Azure Functions
- Azure Blob Storage
- PostgreSQL (Supabase)
- GitHub Actions / Azure DevOps

## Status
Project setup and architecture definition (in progress)
