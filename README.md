# Allora Network Worker Node -EARN BY ABHI

**Use One Click Command** 👇🏻



**Copy Code Below - To Start Worker Node:**
```
wget https://raw.githubusercontent.com/dxzenith/allora-worker-node/main/allora.sh && chmod +x allora.sh && ./allora.sh

```

**Check Your Node Code ( 1 ):**
```
docker ps
docker logs -f <CONTAINER ID>

```

**Check Your Node Code ( 2 ):**
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

**Restart Command For Free Users ( 3 ):**
```
./allora.sh

```

👉🏻**Join Our Telegram:** https://t.me/EarnByAbhi23

👉🏻**Follow Our Twitter:** https://x.com/EarnByAbhi
