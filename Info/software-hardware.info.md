# Homelab Übersicht

=== Wichtige Hardware- und Software-Informationen ===

---

### **Systeminformationen**
- **Betriebssystem**: Debian GNU/Linux 12 (bookworm)
- **Kernel**: Linux 6.8.12-8-pve (SMP PREEMPT_DYNAMIC, 2025-01-24)
- **Hostname**: pve
- **Architektur**: x86_64
- **Uptime**: 8 Stunden, 57 Minuten (Stand: 09. März 2025)

---

### **CPU-Informationen**
- **Modell**: AMD Ryzen 7 5825U mit Radeon Graphics
- **Kerne/Threads**: 8 Kerne, 16 Threads
- **Taktfrequenz**: Variabel zwischen 400 MHz und 4516 MHz (abhängig von Last)
- **Cache**: 512 KB
- **Aktuelle Auslastung**: 9,1 %

---

### **RAM-Informationen**
- **Gesamt**: 62 GiB
- **Verwendet**: 3,0 GiB
- **Frei**: 56 GiB
- **Verfügbar**: 59 GiB
- **Swap Gesamt**: 8,0 GiB
- **Swap Verwendet**: 0 B (vollständig frei)

---

### **Festplatten und Speichergeräte**
1. **/dev/sda** (HDD/SSD):
   - **Größe**: 465,8 GiB
   - **Partitionen**:
     - sda1: 200 MiB (vfat)
     - sda2: 465,4 GiB
2. **/dev/sdb** (vermutlich USB):
   - **Größe**: 480 MiB
   - **Partition**: sdb1 (vfat)
3. **/dev/nvme0n1** (NVMe SSD):
   - **Größe**: 931,5 GiB
   - **Partitionen**:
     - nvme0n1p2: 1 GiB (/boot/efi, vfat)
     - nvme0n1p3: 930,5 GiB (LVM2_member)
       - pve-swap: 8 GiB (swap)
       - pve-root: 96 GiB (/, ext4)
       - pve-data: 100 GiB (LVM)

- **Speicherplatz**:
  - `/dev/mapper/pve-root`: 94 GiB (6,8 GiB benutzt, 83 GiB frei, 8 % Auslastung)
  - `/boot/efi`: 1022 MiB (12 MiB benutzt, 1011 MiB frei)

---

### **Netzwerkinformationen**
- **Aktive Schnittstellen**:
  - **vmbr0**: 192.168.178.38/24 (Gateway: 192.168.178.1)
  - **tailscale0**: 100.65.29.39/32 (VPN)
  - **lo**: 127.0.0.1/8
- **Inaktive Schnittstellen**: enp3s0, enx00e04c682316, docker0
- **Netzwerkverkehr (eno1)**:
  - Empfangen: 1,12 GiB (1.023.821 Pakete)
  - Gesendet: 82,4 MiB (443.368 Pakete)

---

### **Software-Informationen**
- **Kernel-Version**: 6.8.12-8-pve
- **Wichtige Pakete**:
  - Apache: 2.4.62
  - Docker: 28.0.1
  - Python: 3.11.2
  - Bash: 5.2.15
- **Laufende Dienste (Auswahl)**:
  - apache2, docker, containerd, corosync, cron
- **Top-Prozesse (CPU)**:
  - /root/.vscode/cli: 5,1 %
  - /usr/sbin/tailscaled: 1,5 %
  - /usr/sbin/corosync: 0,6 %

---
