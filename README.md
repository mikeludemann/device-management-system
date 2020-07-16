# device-management-system

A simple device management system

## Setup

**Prerequisites**

* NodeJS
* MongoDB

**Installation**

```sh
$ npm install
```

**Create .env file**

```
NODE_ENV=DEVELOPMENT
MONGODB_URL=mongodb://localhost:27017/dms
SESSION_COOKIE_SECRET=<keyboard cat>
DATE_TIME_FORMAT="YYYY-MM-DD HH:mm"

; OAUTH Github
GITHUB_CLIENT_ID=<ID>
GITHUB_CLIENT_SECRET=<SECRET>
GITHUB_CALLBACK=<HOSTNAME>/users/auth/github/callback

; OAUTH Google
GOOGLE_CLIENT_ID=<ID>
GOOGLE_CLIENT_SECRET=<SECRET>
GOOGLE_CALLBACK=<HOSTNAME>/users/auth/google/callback
GOOGLE_HOSTED_DOMAIN=example.com

; AWS S3 for media storage
AWS_ACCESS_KEY_ID=<ID>
AWS_SECRET_ACCESS_KEY=<SECRET>
AWS_MEDIA_BUCKET=<MEDIA-BUCKET>

; Mails settings
MAIL_TRANSPORT=SMTP
MAIL_SERVICE=Gmail
MAIL_USERNAME=
MAIL_PASSWORD=
MAIL_RECIPIENT=<email for system mails>
MAIL_FROM='Admin <admin@mail.com>'
```

**Start**

```sh
$ node app.js
```

Open http://127.0.0.1:3000