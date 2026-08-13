# vpn-amneziawg-server
Secure Linux VPN server based on AmneziaWG 2.0 with server hardening, network configuration, traffic obfuscation, NAT, firewall rules and connectivity diagnostics.

# Secure AmneziaWG VPN Server
## What I Did
- deployed Ubuntu server
- configured AmneziaWG 2.0
- configured routing and NAT
- hardened SSH
- configured firewall
- configured DNS
- enabled IP forwarding
- implemented traffic obfuscation
- tested connectivity and routing

## Architecture

                Internet
                    │
                    │
              UDP / VPN
                    │
                    ▼
        ┌──────────────────────┐
        │   Ubuntu 22.04 VPS   │
        │                      │
        │  AmneziaWG 2.0       │
        │  Firewall            │
        │  NAT                 │
        │  IP Forwarding       │
        │  systemd             │
        │  DNS configuration   │
        └──────────┬───────────┘
                   │
              VPN tunnel
                   │
                   ▼
            ┌────────────┐
            │   Client   │
            │ Android /  │
            │ Linux      │
            └────────────┘

## Technologies
- Ubuntu
- WireGuard
- AmneziaWG 2.0
- iptables
- systemd
- SSH
- DNS
- UFW
- Fail2Ban


# Проект: Личный AmneziaWG VPS 

# Цель:
Развернуть собственный VPN-сервер на Ubuntu VPS с использованием AmneziaWG 2.0.

Что реализовано:
- обновление Ubuntu
- настройка SSH
- изменение порта SSH
- настройка UFW
- настройка Fail2Ban
- установка AmneziaWG 2.0
- настройка двух клиентов
- проверка подключения
- тестирование работы VPN

Используемые технологии:
- Ubuntu
- WireGuard
- AmneziaWG 2.0
- iptables
- systemd
- SSH
- DNS
- UFW
- Fail2Ban
