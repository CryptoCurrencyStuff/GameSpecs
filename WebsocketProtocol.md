# Websocket protocols

### Game

##### Register
```
{ "register": { 
  "name": "Username",
  "password: "secret123"
} }
```

##### Login

request:
```
{ "login": { 
  "name": "Username",
  "password: "secret123",
  "2fa_code": 102837
} }
```

response:
```
{"login":{"success":true,"token":"c51a5d55d0c5fe9ade0c4a1a97a56f43"}}"
```

##### Logout
```
{ "logout": { } }
```

##### Game Configuration
request:
```
{ "config": { } }
```

response:
```
{"config":{"success":true,"precision_digits":10,"min_wager":0,"dynamic_max_profit":false,"dynamic_max_profit_percent":1.000000,"max_profit":1000000,"min_win_chance":0.100000,"max_win_chance":99.000000,"dynamic_house_edge":false,"house_edge_percent":0.000000}}
```

##### Game Stats
```
{ "stats": { } }
```

##### Account Info
```
{ "user_info": { }
```

##### Account Stats
```
{ "user_stats": { 
  "user": "LongCrab" 
} }
```

##### Bet Info
```
{ "bet_info": { 
  "bet_id": 1234567 
} }
```

##### Roll
```
{ "roll": { 
  "amount": 100000,
  "target": 4950,
  "condition_high": false
} }
```
##### Set Seed
```
{ "set_seed": { 
  "client_key": "28JdhjdG7T1LK0",
} }
```

##### Reveal Seed
```
{ "reveal_seed": { } }
```
##### Current Seed Info
```
{ "curr_seed_info": { } }
```

##### Previous Seed Info
```
{ "prev_seed_info": { } }
```

##### Tip
```
{ "tip": {
  "user": "LongCrab",
  "amount": 666666,
  "is_public": false
} }
```

### Chat
