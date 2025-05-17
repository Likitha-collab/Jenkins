# File: .github/workflows/develop-pipeline.yml
name: Develop Branch Pipeline

on:
  push:
    branches:
      - develop

jobs:
  pull-code:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout code
        uses: actions/checkout@v3

      - name: Pull Git content to a folder
        run: |
          mkdir -p pulled_code
          cp -r . pulled_code/
          echo "Code copied to pulled_code folder"
