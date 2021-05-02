## BS-API

Get Your BrawlStars Stats With [`bs-api`](https://cr.is-a.dev)


### Directory 

- [`/`](https://cr.is-a.dev) Home
   - `/:TAG` Players

- [`/brawlers/:TAG`](https://cr.is-a.dev/brawlers/TAG) Get A Player's Brawlers 
 
- [`/support/:CODE`](https://cr.is-a.dev/support/) Content Creator Code

- [`/clubs/:TAG`](https://cr.is-a.dev/clubs`) Clubs

- [`/rankings/`](https://cr.is-a.dev/rankings/) Rankings
  - [`/rankings/clubs/:CODE`](https://cr.is-a.dev/rankings/clubs/) Clubs
  - [`/rankings/players/:CODE`](https://cr.is-a.dev/rankings/players/) Players

- [`/add/:TAG?code=PASSWORD`](https://cr.is-a.dev/add?code=) Add A Player

- [`/v1`](https://cr.is-a.dev/v1) Version 1.0.0
  - [`/v1/brawlers`](https://cr.is-a.dev/v1/brawlers) List Of Every Brawlers ( StarPowers, Gadgets )
  - `/v1/brawlers/:ID` Specific Brawler's Information
  - [`/v1/battlelog/:TAG`](https://cr.is-a.dev/v1/battlelog/) Player's Battlelog
  
 ### Websocket
 
  *  Websocket - `wss://wscr.is-a.dev`
  
  *   ``` Send A Tag To The Server => Response Data To The Client```

```
Example :
const WebSocket = require('ws')
const ws = new WebSocket('wss://wscr.is-a.dev');
ws.onopen = function open() {
  console.log('connected');
  ws.send('8CYPU2VLG');
};
 ws.onmessage = function incoming(message) {
   console.log(JSON.parse(message.data))
};
```
     
  
### About 
  
  Bs-api known as Brawl Stars Stats API is a service where you can get your brawlstars stats easily. Feel Free To Create An Issue If You Have Any Suggestions Or Questions.
  
  
  
  ### Disclaimer 
  
  This Project Was Made By A Fan Of Supercell Games And Not Affiliate With Supercell Or Brawl Stars. This Project Was Managed And Owned By [`@brawlie Team`](https://github.com/brawlie). This Is Not An Official API From Brawl Stars. Made For Education Propose.
  
  
  
  ### License 
  
  ``` 
  APACHE 2.0 License
  ```
  


 
