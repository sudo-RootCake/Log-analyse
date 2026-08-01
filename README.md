# Nginx Log Analyser

Uma ferramenta de linha de comando em Bash para analisar logs de acesso do Nginx.

## Funcionalidades

* Mostra os 5 IPs com mais requisições.
* Mostra os 5 caminhos mais requisitados.
* Mostra os 5 códigos de status HTTP mais frequentes.

## Requisitos

* Bash
* awk
* sort
* uniq
* head

## Como usar

Dê permissão de execução ao script:

```bash
chmod +x log-analyser
```

Execute:

```bash
./log-analyser
```

O arquivo `nginx-access.log` deve estar no mesmo diretório do script.

## Exemplo

```text
Top 5 IP addresses with the most requests:
178.128.94.113 - 1087 requests
142.93.136.176 - 1087 requests
138.68.248.85 - 1087 requests

Top 5 most requested paths:
/v1-health - 4560 requests
/ - 270 requests
/v1-me - 232 requests

Top 5 response status codes:
200 - 5740 requests
404 - 937 requests
304 - 621 requests
```

Projeto inspirado no desafio do roadmap.sh:
https://roadmap.sh/projects/nginx-log-analyser
