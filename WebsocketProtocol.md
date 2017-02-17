# Websocket protocols

## Game

### Register
```
{ "register": { 
  "name": "Username",
  "password: "secret123"
} }
```

#### Login

##### request
```
{ "login": { 
  "name": "Username",
  "password: "secret123",
  "2fa_code": 102837
} }
```

##### response:
```
{"login":{"success":true,"token":"c51a5d55d0c5fe9ade0c4a1a97a56f43"}}"
```

#### Logout
```
{ "logout": { } }
```

#### Game Configuration
##### request
```
{ "config": { } }
```

##### response
```
{"config":{"success":true,"precision_digits":10,"min_wager":0,"dynamic_max_profit":false,"dynamic_max_profit_percent":1.000000,"max_profit":1000000,"min_win_chance":0.100000,"max_win_chance":99.000000,"dynamic_house_edge":false,"house_edge_percent":0.000000}}
```

#### Game Stats
##### request
```
{ "stats": { } }
```

##### response
```
{"stats":{"success":true,"total_bets":210,"total_wins":117,"total_losses":93,"total_wagered":66510000,"total_profit":-2230000.000000,"day_bets":0,"day_wins":0,"day_losses":0,"day_wagered":0,"day_profit":0.000000}}
```

#### Account Info
##### request
```
{ "user_info": { }
```

##### response
```
{"user_info":{"success":true,"username":"asdf22","uid":1,"curr_key_hash":"dc30c107b1f95c74ec1b5b1f8ff4e1b16fad5f5c7a25c68198e8a4ed76f36996","prev_key_hash":"8473f70c39d1b4abd6de89f39020d92470c92127af81b8d9d4a75ddb5f693ff2","bets":210,"wins":117,"losses":93,"wagered":66510000,"profit":2230000.000000,"balance":102230000.000000}}
```

#### Account Stats
```
{ "user_stats": { 
  "user": "LongCrab" 
} }
```

#### Bet Info
```
{ "bet_info": { 
  "bet_id": 1234567 
} }
```

#### Roll
```
{ "roll": { 
  "amount": 100000,
  "target": 4950,
  "condition_high": false
} }
```
#### Set Seed
```
{ "set_seed": { 
  "client_key": "28JdhjdG7T1LK0",
} }
```

#### Reveal Seed
```
{ "reveal_seed": { } }
```
#### Current Seed Info
##### request
```
{ "curr_seed_info": { } }
```

##### response
```
{"curr_seed_info":{"success":true,"server_key_hash":"dc30c107b1f95c74ec1b5b1f8ff4e1b16fad5f5c7a25c68198e8a4ed76f36996","client_key":"asdasdd","is_active":true}}
```

#### Previous Seed Info
##### request
```
{ "prev_seed_info": { } }
```

##### response
```
{"prev_seed_info":{"success":true,"server_key_hash":"8473f70c39d1b4abd6de89f39020d92470c92127af81b8d9d4a75ddb5f693ff2","server_key":"0c3cfc0abcedf7b40b144cfc8610894085289f7e9de59289ca8ed1054f73078c","client_key":"asdasd"}}
```

#### Tip
```
{ "tip": {
  "user": "LongCrab",
  "amount": 666666,
  "is_public": false
} }
```

### Chat
