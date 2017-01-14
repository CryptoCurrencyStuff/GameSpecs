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
  "password: "secret123"
} }
```

##### Logout
```
{ "logout": { } }
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
### Chat
