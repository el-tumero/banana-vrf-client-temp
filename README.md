# Banana VRF Client Temp
Temporary repo for Banana VRF Client

## How to run

1. Add stake to contract - https://github.com/el-tumero/banana-vrf?tab=readme-ov-file#client - will be more user-friendly soon
2. Wait 3 rounds - https://el-tumero.github.io/banana-vrf-status/
3. Run this commands:
```bash
go get .
go build
./banana-vrf-client-temp -rpc wss://rpc.eu-central-1.gateway.fm/ws/v4/lukso/non-archival/testnet -chain_id 4201 -contract D061CEb1F6BE5b6822762893e229FFce5C62C283 -priv <priv_key> -relay 209.38.204.206:3333
```

- rpc - rpc address (websockets)
- chain_id - chain id of dest chain
- contract - VRFHost address - D061CEb1F6BE5b6822762893e229FFce5C62C283
- priv - private key of EOA (in hex string [without 0x])
- relay - address of websocket message relay (we host 209.38.204.206:3333)

## More info
https://github.com/el-tumero/banana-vrf/tree/main