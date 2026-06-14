import requests

TOKEN = "TON_TOKEN"
CHAT_ID = "TON_CHAT_ID"

def send_message(text):
    url = f"https://api.telegram.org/bot{TOKEN}/sendMessage"

    requests.post(url, data={
        "chat_id": CHAT_ID,
        "text": text
    })

TOKEN = "8971163025:AAEtx4V9t5Fdhw3AM-t8lAaAQojq_1DGjIc"
CHAT_ID = "8971163025"

url = f"https://api.telegram.org/bot{TOKEN}/sendMessage"

data = {
    "chat_id": CHAT_ID,
    "text": "TEST MESSAGE"
}
