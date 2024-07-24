# RC Python Quick Start

Ref: https://developers.ringcentral.com/guide/notifications/websockets/quick-start#python

First of all, create a new folder to hold the project:
```shell
mkdir rc-python-quick-start
cd rc-python-quick-start
```

Then, create a new virtual environment:
```shell
python3 -m venv venv
```

Activate the virtual environment:
```shell
source venv/bin/activate
```
You need to run the above command every time you open a new terminal window.

Install the required packages:
```shell
pip install ringcentral python-dotenv
```

Create a new file named `.env` in the project folder, and add the following content:
```dotenv
RC_CLIENT_ID=xxx
RC_CLIENT_SECRET=yyy
RC_JWT=zzz
RC_SERVER_URL=https://platform.ringcentral.com
```
You need to replace `xxx`, `yyy`, and `zzz` with your own RingCentral app client ID, client secret, and JWT token.

Create a new file named `websocket_quick_start.py` in the project folder, and copy paste content from https://developers.ringcentral.com/guide/notifications/websockets/quick-start#python

Run the script:
```shell
python websocket_quick_start.py
```

You should see the script print out:
```
New WebSocket connection created:
```

Upon receiving a new message, you should see the script print out:
```
Subscription notification:
```
