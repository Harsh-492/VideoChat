# DEEPCHAT

## Description 
Video calling application using the Agora Web SDK with a Django backend.

##  How to use this source code

#### 1 - Clone repo
```
git clone https://github.com/Deepakpariharr/DEEPCHAT
```

#### 2 - Install requirements
```
cd DEEPCHAT
pip install -r requirements.txt
```

#### 3 - Update Agora credentals
In order to use this project you will need to replace the agora credentials in `views.py` and `streams.js`.

Create  account at agora.io and create an `app`. Once you create your app, you will want to copy the `appid` & `appCertificate` to update `views.py` and `streams.js`. 


###### views.py
```
def getToken(request):
    appId = "YOUR APP ID"
    appCertificate = "YOUR APPS CERTIFICATE"
    ......
```

###### streams.js
```
....
const APP_ID = 'YOUR APP ID'
....
```


#### 4 - Start server
```
python manage.py runserver
```

