## Git
**Clone from GitHub**
```
git clone [https://xxx.git]
```

## Google App Engine
**Build and run**
```
dev_appserver.py ./
```
```
http://localhost:8080/
```

**Deploy**
```
gcloud app deploy app.yaml index.yaml
```

**Deplay with optional flags**
```
--project [YOUR_PROJECT_ID]
```
```
-v [YOUR_VERSION_ID]
```

#####View deployed application
```
http://[YOUR_PROJECT_ID].appspot.com
```
```
gcloud app browse
```
