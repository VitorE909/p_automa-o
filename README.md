name: Olá Mundo Action

on:
  push:
    branches: [ main ]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Checar código
        uses: actions/checkout@v4

      - name: Rodar Olá Mundo
        run: echo "Olá, mundo!"
