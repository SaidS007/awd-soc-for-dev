# SOC minimal - docker-compose pour déploiement via Dokploy

Contient:
- docker-compose.yml (services Traefik, OpenSearch, TheHive, Wazuh, Postgres, Prometheus, Grafana, Minio, ...)
- prometheus/prometheus.yml

Usage local:
- docker-compose up -d
- docker-compose logs -f <service>

Notes:
- TLS est géré par la plateforme Dokploy / Traefik frontal.
- Pour Postgres, si tu veux conserver d'anciennes données, faire un backup avant de changer d'image.
