#!/bin/bash
set -e

# Install make, curl, unzip if not present
apt-get update && apt-get install -y make curl unzip

# Clone Drosera if not already cloned
if [ ! -d "Drosera-Network" ]; then
  git clone https://github.com/0xmoei/Drosera-Network.git
fi

cd Drosera-Network

# Build binary (sesuai instruksi build dari repo)
make build || go build -o drosera ./cmd/drosera

echo "✅ Drosera Network setup complete!"
