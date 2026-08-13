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
