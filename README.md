# VideoChat App

This project is a Video Conference website, comprising 3 in-call functionalities (mute, video on/off, and end-call)

## How to use

In order to use this project you will need to replace the agora credentials in `views.py` and `streams.js` files.

Create an account at agora.io and create an app. Once you create your app, you will want to copy the appid & appCertificate to update `views.py` and `streams.js`

In the `views.py` file, make the update at the following location:

```
def getToken(request):
    appId = "YOUR APP ID"
    appCertificate = "YOUR APPS CERTIFICATE"
    ......
```

Also, make the change in the `streams.js` file as follows:

```
....
const APP_ID = 'YOUR APP ID'
....
```

Now you are ready! To start the app, run the following command in your prompt:

```
python manage.py runserver
```
