## Adding rewards:

import requests
import json

payload = {"name": "klarps", "reward": 3}
response = requests.post('https://8gx25z-5000.csb.app/rewards', json=payload)
print(response.text)

## Getting Rewards
import requests
import json

payload = {"name": "klarps"}
response = requests.post('/v1/chat/currency', json=payload)
print(response.text)

## Add Items
import requests
import json

payload = {"name": "klarps", "item": "sword}
response = requests.post('https://8gx25z-5000.csb.app/API', json=json.dumps(payload))
print(response.text)
