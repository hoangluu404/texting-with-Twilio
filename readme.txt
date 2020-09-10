install python plugins
py -m pip install PLUGINS

trial phone number +12058983132
ACCOUNT SID ACe42ad7f3392d08ac140f1ae2d17ce1b0
AUTH TOKEN 32fffbfe27ac45a22353675b5db8d4fa


# Send an SMS Using Twilio
# Download the helper library from https://www.twilio.com/docs/python/install
from twilio.rest import Client


# Your Account Sid and Auth Token from twilio.com/console
For secure See http://twil.io/secure
account_sid = 'ACe42ad7f3392d08ac140f1ae2d17ce1b0'
auth_token = 'your_auth_token'
text = input("Enter a Text Message: ")
client = Client(account_sid, auth_token)

message = client.messages \
                .create(
                     body = text,
                     from_='+12058983132',
                     to='+18177688888'
                 )
print(message.sid)





# EXCEL
import openpyxl
wb = openpyxl.load_workbook(file)
sheet = wb['Sheet1']
sheet.cell(row=#,column=#).value



JSON response to message -> message.sid, message.date_created...
{"sid": "SMxxxxxxxxxxxxxxx", 
 "date_created": "Thu, 09 Aug 2018 17:26:08 +0000", 
 "date_updated": "Thu, 09 Aug 2018 17:26:08 +0000", 
 "date_sent": null, 
 "account_sid": "ACxxxxxxxxxxxxxxxx", 
 "to": "+15558675310",
 "from": "+15017122661",
 "messaging_service_sid": null,
 "body": "This is the ship that made the Kessel Run in fourteen parsecs?", 
 "status": "queued", 
 "num_segments": "1", 
 "num_media": "0",
 "direction": "outbound-api",
 "api_version": "2010-04-01",
 "price": null,
 "price_unit": "USD",
 "error_code": null,
 "error_message": null,
 "uri": "/2010-04-01/Accounts/ACxxxxxxxxx/Messages/SMxxxxxxxxxxxx.json",
 "subresource_uris": {
     "media": null
 }
}