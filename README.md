## Git
**Create a Project**
```
$ git init myproject
$ cd myproject
$ git add .
$ git commit -m"importing all codes"
```

**Work on Same Project**
```
alice $ git checkout master
alice $ git commit -a -m"alice's update"
alice $ git push
```
```
bob $ git checkout -b afork
bob $ git commit -a -m"bob's update"
bob $ git push origin afork
```
```
bob $ git push
bob $ git merge afork
```

**Partial Update**
```
$ git add -p samplefile.swift
$ git commit -m"sample comment"
```

**Find Remote Origin**
```
$ git config --get remote.origin.url
```

**Change Remote Origin**
```
$ git remote -v
$ git remote set-url origin https://github.com/USERNAME/REPOSITORY.git
```


**Clone from GitHub**
```
$ git clone [https://xxx.git]
```

**History Graph**
```
$ git log --graph --decorate --abbrev-commit --all -pretty=oneline
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

**Deploy with optional flags**
```
--project [YOUR_PROJECT_ID]
```
```
-v [YOUR_VERSION_ID]
```

**View deployed application**
```
http://[YOUR_PROJECT_ID].appspot.com
```
```
gcloud app browse
```

## Curl
**Test Application**
```
curl -X GET http://localhost:8080/
```
```
curl -X GET http://localhost:8080/user/default/json/
```
```
curl -X POST -H "Content-Type: multipart/form-data" -F caption='curl' -F "image=@kitten.jpg" http://localhost:8080/post/lolakitty/
```
