# admin-scripts

A few bash scripts for OrganiCity

## oc-token

usage : ```oc-token client_login client_password```

Requests an access token on the authentication SERVEUR using client credentials

## oc-addrole

usage : ```oc-addrole client_login client_password userSub roleName```

Requests an access token on the authentication SERVEUR using client credentials, then gives a user (using its related userSub) the role roleName.

role example : 'manager-dev:site-user'
