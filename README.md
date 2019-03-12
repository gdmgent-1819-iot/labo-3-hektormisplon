## make a web app

```
├───flask
│   ├───templates
│   │   └───environment.html
│   │   └───ambilight.html
│   └───server.py
└───sensehat_dashboard
    ├───assets
    │   ├───css
    │   └───js
    ├───pi
    │   └───environment.py
    │   └───ambilight.py
    ├───vendor
    │  └───color-picker
    └───index.html
```

### server-side (flask + firebase)

environment.py: on specified interval send values of sensors to firebase

ambilight.py: server listens for firebase updates

### client-side (dashboard)

listens to changes in environment file in firebase

sends changes from ambilight to firebase
