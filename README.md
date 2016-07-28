# admin-scripts

A few bash scripts for OrganiCity.

Required packages
 * curl : the well known command-line HTTP client
 * jq : lightweight and flexible command-line JSON processor

## 1. Scripts for role management

### 1.1 oc-token

usage : ```oc-token client_login client_password```

Requests an access token on the authentication SERVEUR using client credentials

### 1.2 oc-getrole

usage : ```oc-getroles client_login client_password userSub```

Requests an access token on the authentication SERVEUR using client credentials, then gets the list of a user (using its related userSub) roles.

### 1.3 oc-addrole

usage : ```oc-addrole client_login client_password userSub roleName```

Requests an access token on the authentication SERVEUR using client credentials, then gives a user (using its related userSub) the role roleName.

role example : 'manager-dev:site-user'

## 2. misc

### 2.1 checkRunning

...
