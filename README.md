# admin-scripts

A few bash scripts for OrganiCity.

Required packages
 * curl : the well known command-line HTTP client
 * jq : lightweight and flexible command-line JSON processor


## oc-token

usage : ```oc-token client_login client_password```

Requests an access token on the authentication SERVEUR using client credentials

## oc-getrole

usage : ```oc-getroles client_login client_password userSub```

Requests an access token on the authentication SERVEUR using client credentials, then gets the list of a user (using its related userSub) roles.

## oc-addrole

usage : ```oc-addrole client_login client_password userSub roleName```

Requests an access token on the authentication SERVEUR using client credentials, then gives a user (using its related userSub) the role roleName.

role example : 'manager-dev:site-user'
