# admin-scripts

A few bash scripts for OrganiCity.

Required packages
 * curl : the well known command-line HTTP client
 * jq : lightweight and flexible command-line JSON processor

## 1. General purpose scripts

### 1.1 oc-token

usage : ```oc-token client_login client_password```

Requests an access token on the authentication SERVEUR using client credentials

### 1.2 oc-getusers

usage : ```oc-getusers client_login client_password```

Requests an access token on the authentication SERVEUR using client credentials, then gets the list of all the users subs and names.


## 2. Role management scripts


### 2.1 oc-getroles

usage : ```oc-getroles client_login client_password userSub```

Requests an access token on the authentication SERVEUR using client credentials, then gets the list of a user (using his/her related userSub) roles.

### 2.2 oc-addrole

usage : ```oc-addrole client_login client_password userSub roleName```

Requests an access token on the authentication SERVEUR using client credentials, then gives a user (using his/her related userSub) the role roleName.

role example : 'manager-dev:site-user'

### 2.3 oc-removerole

usage : ```oc-removerole client_login client_password userSub roleName```

Requests an access token on the authentication SERVEUR using client credentials, then remove a role to a user identified by his/her sub.

### 2.3 oc-addroletoall

usage : ```oc-addroletoall client_login client_password roleName```

Requests an access token on the authentication SERVEUR using client credentials, then gives all users the role roleName

role example : 'manager-dev:site-user'

## 2. misc

### 2.1 checkRunning

...
