# Llama2-api-free
Llama2 unofficial api reverse engineered!
This repository contains Llama2 70b reverse engineered api 

# how to use? 
Using Llama2 reversed engineered api is very easy follow these steps! 

# 1st join our discord 
https://discord.gg/BsunT6jhT
## Prerequisites
- Python 3.8 or higher
- Windows, macOS, or Linux operating system

  ## 2nd use!
```import requests
import json

url = "https://www.llama2.ai/api"
headers = {
  "Content-Type": "application/json",
  "Origin": "https://www.llama2.ai",
  "Referer": "https://www.llama2.ai/",
  "User-Agent": "Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/119.0.0.0 Mobile Safari/537.36"
}

payload = {
  "prompt": "hi ",
  "systemPrompt": "you are an awesome intelligent Chatbot made by Ionium AI xD ",
  "temperature": 2,
  "topP": 0.6,
  "version": "02e509c789964a7ea8736978a43525956ef40397be9033abf9fd2badfe68c9e3",
  "maxTokens": 18000
}

response = requests.post(url, headers=headers, data=json.dumps(payload))

print(response.text)

try:
   data = response.json()
   print(data)
except json.JSONDecodeError:
   print("Failed to decode JSON")
```
