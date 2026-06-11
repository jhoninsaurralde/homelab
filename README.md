<<<<<<< HEAD
# homelab
Home lab server build — Ubuntu Server, Docker, self-hosted services
=======
# Homelab

Servidor casero construido sobre hardware de bajo costo con foco en privacidad, self-hosting y aprendizaje de infraestructura Linux.

## Hardware

- **Notebook:** Pentium T4500, 4GB RAM
- **OS:** Ubuntu Server 24.04 LTS
- **Almacenamiento:** HDD 320GB (OS) + HDD 320GB (datos, montado en /mnt/raid)
- **Red:** WiFi Realtek, IP estática 192.168.0.100

## Stack

| Servicio | Descripción | Puerto |
|---|---|---|
| Pi-hole | Bloqueo de publicidad y rastreo a nivel DNS | 80 |
| Portainer | Gestión de contenedores Docker | 9000 |
| Gitea | Repositorio Git self-hosted | 3000 |
| Filebrowser | Gestor de archivos web | 8082 |
| Netdata | Monitoreo del servidor en tiempo real | 19999 |
| Homarr | Dashboard central de servicios | 7575 |
| Whoogle | Buscador privado basado en Google | 5000 |
| Privoxy | Proxy HTTP para dispositivos legacy | 8118 |

## Bot de Telegram

Bot personal con IA (Groq LLaMA 3.3 70B) integrado al servidor con:
- Historial de conversación persistente
- Búsqueda web automática
- OCR para extracción de texto en imágenes

## Infraestructura

- Docker + Docker Compose para orquestación de servicios
- systemd para servicios nativos (Gitea, bot de Telegram)
- IP estática configurada via Netplan
- Almacenamiento secundario montado y persistente
>>>>>>> 3a4105f (Initial homelab documentation)
