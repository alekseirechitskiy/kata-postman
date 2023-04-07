# kata-postman - 4.4.9
### 1. Registration

POST:
```
  "user": {
    "username": "AlexeiRechitskiy",
    "email": "slow_spirit@gmail.com",
    "password": "pasS-Word"
  }
}
```
Response:
```
{
    "user": {
        "username": "alexeirechitskiy",
        "email": "slow_spirit@gmail.com",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY0MzAwNjAyNjBjNjc1MWIwMGI3NGMwYiIsInVzZXJuYW1lIjoiYWxleGVpcmVjaGl0c2tpeSIsImV4cCI6MTY4NjA1Mjg2NiwiaWF0IjoxNjgwODY4ODY2fQ.zLII0XyDzUD4k15sYxoIiU_4414Nc8oY7FluJLuvIDw"
    }
}
```
### 2. Login
POST:
```
{
  "user": {
    "email": "slow_spirit@gmail.com",
    "password": "pasS-Word"
  }
}
```
Response:
```
{
    "user": {
        "username": "alexeirechitskiy",
        "email": "slow_spirit@gmail.com",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY0MzAwNjAyNjBjNjc1MWIwMGI3NGMwYiIsInVzZXJuYW1lIjoiYWxleGVpcmVjaGl0c2tpeSIsImV4cCI6MTY4NjA1MzEzMCwiaWF0IjoxNjgwODY5MTMwfQ.kRFqZ3R5p3hsBMogEeitF456ReA9fIKOra81jc-l56s"
    }
}
```

### 3. Get current
GET:
```
https://blog.kata.academy/api/user?email=slow_spirit@gmail.com&token=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY0MzAwNjAyNjBjNjc1MWIwMGI3NGMwYiIsInVzZXJuYW1lIjoiYWxleGVpcmVjaGl0c2tpeSIsImV4cCI6MTY4NjA1MzEzMCwiaWF0IjoxNjgwODY5MTMwfQ.kRFqZ3R5p3hsBMogEeitF456ReA9fIKOra81jc-l56s&username=alexeirechitskiy
```
Response:
```
{
    "user": {
        "username": "alexeirechitskiy",
        "email": "slow_spirit@gmail.com",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY0MzAwNjAyNjBjNjc1MWIwMGI3NGMwYiIsInVzZXJuYW1lIjoiYWxleGVpcmVjaGl0c2tpeSIsImV4cCI6MTY4NjA1NDgwMywiaWF0IjoxNjgwODcwODAzfQ.bvqKupoSEUQ0mlIscH1wxGQ707SWr0dCKUH-RAp7jDk"
    }
}
```
