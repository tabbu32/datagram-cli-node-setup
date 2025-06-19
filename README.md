# datagram-cli-node-setup
Step-by-step guide to run Datagram CLI node on a VPS (Google Cloud, Contabo, etc.)
# Datagram VPS Node Setup (Linux)

This repo contains a step-by-step guide to run the Datagram CLI node on your Linux VPS.

---

## ✅ Requirements

- Ubuntu 20.04 / 22.04
- At least 2 vCPU, 4GB RAM, 20GB SSD
- Root or sudo access

---

## 📦 Installation

```bash
# 1. Download
wget https://github.com/Datagram-Group/datagram-cli-release/releases/latest/download/datagram-cli-x86_64-linux -O ~/datagram

# 2. Make it executable
chmod +x ~/datagram

# 3. Move to ~/.local/bin
mkdir -p ~/.local/bin
mv ~/datagram ~/.local/bin/datagram

# 4. Add to PATH
echo 'export PATH=$HOME/.local/bin:$PATH' >> ~/.bashrc
source ~/.bashrc
