## Adding rewards:

```
import requests
import json

payload = {"name": "klarps", "reward": 3}
response = requests.post('https://8gx25z-5000.csb.app/v1/chat/rewards', json=payload)
print(response.text)
```

## Getting Rewards
```
import requests
import json

payload = {"name": "klarps"}
response = requests.post('https://8gx25z-5000.csb.app/v1/get/currency', json=payload)
print(response.text)
```
## Add Items
```
import requests
import json

payload = {"name": "klarps", "item": {"name": "sword", "item_info": "info"}}
response = requests.post('https://8gx25z-5000.csb.app/v1/chat/items', json=payload)
print(response.text)
```
## Game Win
```
import requests
import json

payload = {"name": "klarps", "reward": 500, "score": 500, "game": "Game"}
response = requests.post('https://8gx25z-5000.csb.app/v1/chat/gamewin', json=payload)
print(response.text)
```
## Scoreboard
```
import requests
import json

payload = {"game": "TicaTacToe"}
response = requests.post('https://8gx25z-5000.csb.app/v1/get/scoreboard', json=payload)
print(response.text)
```
## Add Item to Shop
```
import requests

item = requests.get("https://store.ncss.cloud/group2/shop").json()
attributes = {"url": "", "price": 500}
item["wallpaper"] = attributes
requests.post("https://store.ncss.cloud/group2/shop", json=item)
```

