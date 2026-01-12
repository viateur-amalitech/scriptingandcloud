# Lab 1: YAML Configuration

## Overview
This lab demonstrates how to create and validate YAML configuration files for a sample web application.

## Files
- `app-config.yaml`: The primary configuration file in YAML format.
- `app-config.json`: The converted configuration file in JSON format.

## Content
### app-config.yaml
```yaml
application:
  name: "my-web-app"
  version: "1.0.0"
  environment: "production"
server:
  host: "0.0.0.0"
  port: 8080
database:
  engine: "mysql"
  host: "db.example.com"
  port: 3306
  username: "admin"
  password: "mysecurepassword"
```

## Steps Completed
1. Created `app-config.yaml` with the defined structure.
2. Validated the YAML syntax using `yamllint`.
3. Converted YAML to JSON using `yq`.

## How to convert & validate 
```bash
# Validate YAML syntax
yamllint app-config.yaml

# Convert YAML to JSON
yq . app-config.yaml > app-config.json
```
