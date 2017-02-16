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
```
{ "login": { 
  "name": "Username",
  "password: "secret123",
  "2fa_code": 102837
} }
```

##### Logout
```
{ "logout": { } }
```

##### Game Configuration
```
{ "config": { } }
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
