# Allora Network Worker Node -EARN BY ABHI

**Use Commands One By One** 👇🏻



1. **Code For Updating:**
```
sudo apt update && sudo apt upgrade -y \

sudo apt install curl git jq build-essential gcc unzip wget lz4 -y
```

2. **Now Run The Worker:**
```
wget https://raw.githubusercontent.com/dxzenith/allora-worker-node/main/allora.sh && chmod +x allora.sh && ./allora.sh
```

3. **If There Is Any Error , Use Command Below:** ( Optional )
```
sudo usermod -aG docker $USER
```
```
sudo reboot
```

4. **In Next Step , You Need To Enter Keplr Phrase Key & HEAD ID**

5. **Now You Can Check Status:**
```
  curl --location 'http://localhost:6000/api/v1/functions/execute' \
--header 'Content-Type: application/json' \
--data '{
    "function_id": "bafybeigpiwl3o73zvvl6dxdqu7zqcub5mhg65jiky2xqb4rdhfmikswzqm",
    "method": "allora-inference-function.wasm",
    "parameters": null,
    "topic": "1",
    "config": {
        "env_vars": [
            {
                "name": "BLS_REQUEST_PATH",
                "value": "/api"
            },
            {
                "name": "ALLORA_ARG_PARAMS",
                "value": "ETH"
            }
        ],
        "number_of_nodes": -1,
        "timeout": 2
    }
}'
```

6. **Now Lets Migrate Worker Node To V2:**
```
wget -O testnetmigrator.sh https://raw.githubusercontent.com/casual1st/alloraworkersetup/main/testnetmigrator.sh && chmod +x testnetmigrator.sh && ./testnetmigrator.sh
```

👉🏻**Join Our Telegram:** https://t.me/EarnByAbhi23

👉🏻**Follow Us On Twitter:** : https://x.com/EarnByAbhi
