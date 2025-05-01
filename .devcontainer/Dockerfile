# Use Python 3.11 slim base image
FROM python:3.11-slim

# Install system dependencies
RUN apt-get update && apt-get install -y \
    git \
    curl \
    unzip \
    build-essential \
    && rm -rf /var/lib/apt/lists/*

# Install dbt-core and DuckDB adapter
RUN pip install --no-cache-dir dbt-core dbt-duckdb

# Set working directory
WORKDIR /workspace

# Set default command
CMD [ "bash" ]
