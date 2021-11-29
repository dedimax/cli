# API dedimax Bash client

## Overview

This is a Bash client script for accessing API dedimax service.

The script uses cURL underneath for making all REST calls.

## Usage

```shell
# Make sure the script has executable rights
$ chmod u+x 

# Print the list of operations available on the service
$ ./ -h

# Print the service description
$ ./ --about

# Print detailed information about specific operation
$ ./ <operationId> -h

# Make GET request
./ --host http://<hostname>:<port> --accept xml <operationId> <queryParam1>=<value1> <header_key1>:<header_value2>

# Make GET request using arbitrary curl options (must be passed before <operationId>) to an SSL service using username:password
 -k -sS --tlsv1.2 --host https://<hostname> -u <user>:<password> --accept xml <operationId> <queryParam1>=<value1> <header_key1>:<header_value2>

# Make POST request
$ echo '<body_content>' |  --host <hostname> --content-type json <operationId> -

# Make POST request with simple JSON content, e.g.:
# {
#   "key1": "value1",
#   "key2": "value2",
#   "key3": 23
# }
$ echo '<body_content>' |  --host <hostname> --content-type json <operationId> key1==value1 key2=value2 key3:=23 -

# Preview the cURL command without actually executing it
$  --host http://<hostname>:<port> --dry-run <operationid>

```

## Docker image

You can easily create a Docker image containing a preconfigured environment
for using the REST Bash client including working autocompletion and short
welcome message with basic instructions, using the generated Dockerfile:

```shell
docker build -t my-rest-client .
docker run -it my-rest-client
```

By default you will be logged into a Zsh environment which has much more
advanced auto completion, but you can switch to Bash, where basic autocompletion
is also available.

## Shell completion

### Bash

The generated bash-completion script can be either directly loaded to the current Bash session using:

```shell
source .bash-completion
```

Alternatively, the script can be copied to the `/etc/bash-completion.d` (or on OSX with Homebrew to `/usr/local/etc/bash-completion.d`):

```shell
sudo cp .bash-completion /etc/bash-completion.d/
```

#### OS X

On OSX you might need to install bash-completion using Homebrew:

```shell
brew install bash-completion
```

and add the following to the `~/.bashrc`:

```shell
if [ -f $(brew --prefix)/etc/bash_completion ]; then
  . $(brew --prefix)/etc/bash_completion
fi
```

### Zsh

In Zsh, the generated `_` Zsh completion file must be copied to one of the folders under `$FPATH` variable.

## Documentation for API Endpoints

All URIs are relative to */api/3.0*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*CloudApi* | [**cloudterminate**](docs/CloudApi.md#cloudterminate) | **DELETE** /cloud/{id} | Terminate cloud server
*CloudApi* | [**getcloud**](docs/CloudApi.md#getcloud) | **GET** /cloud/{id} | Get cloud informations
*CloudApi* | [**getcloudaddons**](docs/CloudApi.md#getcloudaddons) | **GET** /cloud/addons | Get cloud addons
*CloudApi* | [**getcloudipdetails**](docs/CloudApi.md#getcloudipdetails) | **GET** /cloud/{id}/ips/{ip} | Get cloud ip details
*CloudApi* | [**getcloudips**](docs/CloudApi.md#getcloudips) | **GET** /cloud/{id}/ips | Get cloud ips
*CloudApi* | [**getcloudlocation**](docs/CloudApi.md#getcloudlocation) | **GET** /cloud/location | Get cloud locations
*CloudApi* | [**getcloudplan**](docs/CloudApi.md#getcloudplan) | **GET** /cloud/plan | Get cloud plans
*CloudApi* | [**getcloudreboot**](docs/CloudApi.md#getcloudreboot) | **GET** /cloud/{id}/reboot | Get cloud reboot
*CloudApi* | [**getclouds**](docs/CloudApi.md#getclouds) | **GET** /cloud | Get cloud servers
*CloudApi* | [**getcloudshutdown**](docs/CloudApi.md#getcloudshutdown) | **GET** /cloud/{id}/shutdown | Get cloud shutdown
*CloudApi* | [**getcloudtemplates**](docs/CloudApi.md#getcloudtemplates) | **GET** /cloud/templates | Get cloud templates
*CloudApi* | [**postcloud**](docs/CloudApi.md#postcloud) | **POST** /cloud | Create new cloud server
*CloudApi* | [**postcloudclone**](docs/CloudApi.md#postcloudclone) | **POST** /cloud/{id}/clone | Post cloud clone
*CloudApi* | [**postcloudhostname**](docs/CloudApi.md#postcloudhostname) | **POST** /cloud/{id}/hostname | Post cloud hostname
*CloudApi* | [**postcloudlabel**](docs/CloudApi.md#postcloudlabel) | **POST** /cloud/{id}/label | Post cloud label
*CloudApi* | [**postcloudupgrade**](docs/CloudApi.md#postcloudupgrade) | **POST** /cloud/{id}/upgrade | Upgrade cloud server
*CloudApi* | [**setcloudipreverse**](docs/CloudApi.md#setcloudipreverse) | **POST** /cloud/{id}/ips/{ip}/reverse | Post cloud ip reverse
*CloudApi* | [**setcloudsetup**](docs/CloudApi.md#setcloudsetup) | **POST** /cloud/{id}/setup | Post cloud setup
*DedicatedServerApi* | [**deletededicatedipmi**](docs/DedicatedServerApi.md#deletededicatedipmi) | **DELETE** /dedicatedserver/{id}/ipmi | Delete ipmi access
*DedicatedServerApi* | [**getdedicatedaddon**](docs/DedicatedServerApi.md#getdedicatedaddon) | **GET** /dedicatedserver/{id}/addon | Get dedicated addon
*DedicatedServerApi* | [**getdedicatedhostname**](docs/DedicatedServerApi.md#getdedicatedhostname) | **GET** /dedicatedserver/{id}/hostname | Get dedicated server hostname
*DedicatedServerApi* | [**getdedicatedip**](docs/DedicatedServerApi.md#getdedicatedip) | **GET** /dedicatedserver/{id}/ip | Get dedicated server ip
*DedicatedServerApi* | [**getdedicatedipmi**](docs/DedicatedServerApi.md#getdedicatedipmi) | **GET** /dedicatedserver/{id}/ipmi | Get ipmi access
*DedicatedServerApi* | [**getdedicatedos**](docs/DedicatedServerApi.md#getdedicatedos) | **GET** /dedicatedserver/{id}/os | Get dedicated server os
*DedicatedServerApi* | [**getdedicatedosrescue**](docs/DedicatedServerApi.md#getdedicatedosrescue) | **GET** /dedicatedserver/{id}/rescuetemplates | Get dedicated os rescue
*DedicatedServerApi* | [**getdedicatedplanaddons**](docs/DedicatedServerApi.md#getdedicatedplanaddons) | **GET** /dedicatedserver/plan/{id}/addon | Get dedicated server addons
*DedicatedServerApi* | [**getdedicatedplanos**](docs/DedicatedServerApi.md#getdedicatedplanos) | **GET** /dedicatedserver/plan/{id}/os | Get dedicated server os
*DedicatedServerApi* | [**getdedicatedrescuecredentials**](docs/DedicatedServerApi.md#getdedicatedrescuecredentials) | **GET** /dedicatedserver/{id}/rescuecredentials | Get rescue credentials
*DedicatedServerApi* | [**getdedicatedserver**](docs/DedicatedServerApi.md#getdedicatedserver) | **GET** /dedicatedserver/{id} | Get dedicated server informations
*DedicatedServerApi* | [**getdedicatedserverplan**](docs/DedicatedServerApi.md#getdedicatedserverplan) | **GET** /dedicatedserver/plan | Get dedicated server plans
*DedicatedServerApi* | [**getdedicatedservers**](docs/DedicatedServerApi.md#getdedicatedservers) | **GET** /dedicatedserver | Get dedicated servers
*DedicatedServerApi* | [**postdedicatedboot**](docs/DedicatedServerApi.md#postdedicatedboot) | **POST** /dedicatedserver/{id}/bootnormal | Post dedicated server boot normal mode
*DedicatedServerApi* | [**postdedicatedbootrescue**](docs/DedicatedServerApi.md#postdedicatedbootrescue) | **POST** /dedicatedserver/{id}/bootrescue | Post dedicated server rescue
*DedicatedServerApi* | [**postdedicatedhostname**](docs/DedicatedServerApi.md#postdedicatedhostname) | **POST** /dedicatedserver/{id}/hostname | Post dedicated server hostname
*DedicatedServerApi* | [**postdedicatedipmi**](docs/DedicatedServerApi.md#postdedicatedipmi) | **POST** /dedicatedserver/{id}/ipmi | Create ipmi access
*DedicatedServerApi* | [**postdedicatedipreverse**](docs/DedicatedServerApi.md#postdedicatedipreverse) | **POST** /dedicatedserver/{id}/ip/reverse | Post ip reverse
*DedicatedServerApi* | [**postdedicatedlabel**](docs/DedicatedServerApi.md#postdedicatedlabel) | **POST** /dedicatedserver/{id}/label | Post dedicated server label
*DedicatedServerApi* | [**postdedicatedreboot**](docs/DedicatedServerApi.md#postdedicatedreboot) | **POST** /dedicatedserver/{id}/reboot | Post dedicated server reboot
*DedicatedServerApi* | [**postdedicatedserver**](docs/DedicatedServerApi.md#postdedicatedserver) | **POST** /dedicatedserver | Create dedicated server
*DedicatedServerApi* | [**postdedicatedsetup**](docs/DedicatedServerApi.md#postdedicatedsetup) | **POST** /dedicatedserver/{id}/setup | Setup process
*DedicatedServerApi* | [**postdedicatedshutdown**](docs/DedicatedServerApi.md#postdedicatedshutdown) | **POST** /dedicatedserver/{id}/shutdown | Post dedicated server shutdown
*DedicatedServerApi* | [**terminatededicated**](docs/DedicatedServerApi.md#terminatededicated) | **DELETE** /dedicatedserver/{id} | Terminate dedicated server
*UserApi* | [**getnotifications**](docs/UserApi.md#getnotifications) | **GET** /user/notifications | Get notifications
*UserApi* | [**getuser**](docs/UserApi.md#getuser) | **GET** /user | Get user informations
*UserApi* | [**getwallet**](docs/UserApi.md#getwallet) | **GET** /user/wallet | Get wallet informations


## Documentation For Models

 - [Balance](docs/Balance.md)
 - [Cloud](docs/Cloud.md)
 - [CloudLocation](docs/CloudLocation.md)
 - [DedicatedServer](docs/DedicatedServer.md)
 - [Notification](docs/Notification.md)
 - [OffreCloud](docs/OffreCloud.md)
 - [OffreDedie](docs/OffreDedie.md)
 - [OffreOptionCloud](docs/OffreOptionCloud.md)
 - [OffreOptionDedie](docs/OffreOptionDedie.md)
 - [OsCloud](docs/OsCloud.md)
 - [OsDedie](docs/OsDedie.md)
 - [User](docs/User.md)


## Documentation For Authorization


## BasicAuth

- **Type**: HTTP basic authentication

