## Adding rewards:

import requests
import json

payload = {"name": "klarps", "reward": 3, "task": "add reward"}
response = requests.post('https://8gx25z-5000.csb.app/API', json=json.dumps(payload))
print(response.text)

## Getting Rewards
import requests
import json

payload = {"name": "klarps", "task": "get reward"}
response = requests.post('https://8gx25z-5000.csb.app/API', json=json.dumps(payload))
print(response.text)

## Add Items
import requests
import json

payload = {"name": "klarps", "task": "add items"}
response = requests.post('https://8gx25z-5000.csb.app/API', json=json.dumps(payload))
print(response.text)
