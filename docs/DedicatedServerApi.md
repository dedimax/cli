# DedicatedServerApi

All URIs are relative to */api/3.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deletededicatedipmi**](DedicatedServerApi.md#deletededicatedipmi) | **DELETE** /dedicatedserver/{id}/ipmi | Delete ipmi access
[**getdedicatedaddon**](DedicatedServerApi.md#getdedicatedaddon) | **GET** /dedicatedserver/{id}/addon | Get dedicated addon
[**getdedicatedhostname**](DedicatedServerApi.md#getdedicatedhostname) | **GET** /dedicatedserver/{id}/hostname | Get dedicated server hostname
[**getdedicatedip**](DedicatedServerApi.md#getdedicatedip) | **GET** /dedicatedserver/{id}/ip | Get dedicated server ip
[**getdedicatedipmi**](DedicatedServerApi.md#getdedicatedipmi) | **GET** /dedicatedserver/{id}/ipmi | Get ipmi access
[**getdedicatedos**](DedicatedServerApi.md#getdedicatedos) | **GET** /dedicatedserver/{id}/os | Get dedicated server os
[**getdedicatedosrescue**](DedicatedServerApi.md#getdedicatedosrescue) | **GET** /dedicatedserver/{id}/rescuetemplates | Get dedicated os rescue
[**getdedicatedplanaddons**](DedicatedServerApi.md#getdedicatedplanaddons) | **GET** /dedicatedserver/plan/{id}/addon | Get dedicated server addons
[**getdedicatedplanos**](DedicatedServerApi.md#getdedicatedplanos) | **GET** /dedicatedserver/plan/{id}/os | Get dedicated server os
[**getdedicatedrescuecredentials**](DedicatedServerApi.md#getdedicatedrescuecredentials) | **GET** /dedicatedserver/{id}/rescuecredentials | Get rescue credentials
[**getdedicatedserver**](DedicatedServerApi.md#getdedicatedserver) | **GET** /dedicatedserver/{id} | Get dedicated server informations
[**getdedicatedserverplan**](DedicatedServerApi.md#getdedicatedserverplan) | **GET** /dedicatedserver/plan | Get dedicated server plans
[**getdedicatedservers**](DedicatedServerApi.md#getdedicatedservers) | **GET** /dedicatedserver | Get dedicated servers
[**postdedicatedboot**](DedicatedServerApi.md#postdedicatedboot) | **POST** /dedicatedserver/{id}/bootnormal | Post dedicated server boot normal mode
[**postdedicatedbootrescue**](DedicatedServerApi.md#postdedicatedbootrescue) | **POST** /dedicatedserver/{id}/bootrescue | Post dedicated server rescue
[**postdedicatedhostname**](DedicatedServerApi.md#postdedicatedhostname) | **POST** /dedicatedserver/{id}/hostname | Post dedicated server hostname
[**postdedicatedipmi**](DedicatedServerApi.md#postdedicatedipmi) | **POST** /dedicatedserver/{id}/ipmi | Create ipmi access
[**postdedicatedipreverse**](DedicatedServerApi.md#postdedicatedipreverse) | **POST** /dedicatedserver/{id}/ip/reverse | Post ip reverse
[**postdedicatedlabel**](DedicatedServerApi.md#postdedicatedlabel) | **POST** /dedicatedserver/{id}/label | Post dedicated server label
[**postdedicatedreboot**](DedicatedServerApi.md#postdedicatedreboot) | **POST** /dedicatedserver/{id}/reboot | Post dedicated server reboot
[**postdedicatedserver**](DedicatedServerApi.md#postdedicatedserver) | **POST** /dedicatedserver | Create dedicated server
[**postdedicatedsetup**](DedicatedServerApi.md#postdedicatedsetup) | **POST** /dedicatedserver/{id}/setup | Setup process
[**postdedicatedshutdown**](DedicatedServerApi.md#postdedicatedshutdown) | **POST** /dedicatedserver/{id}/shutdown | Post dedicated server shutdown
[**terminatededicated**](DedicatedServerApi.md#terminatededicated) | **DELETE** /dedicatedserver/{id} | Terminate dedicated server



## deletededicatedipmi

Delete ipmi access

Delete ipmi credentials

### Example

```bash
 deletededicatedipmi id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getdedicatedaddon

Get dedicated addon

Returns dedicated addon

### Example

```bash
 getdedicatedaddon id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]

### Return type

[**array[OffreOptionDedie]**](OffreOptionDedie.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getdedicatedhostname

Get dedicated server hostname

Returns server hostname

### Example

```bash
 getdedicatedhostname id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getdedicatedip

Get dedicated server ip

Returns ip

### Example

```bash
 getdedicatedip id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getdedicatedipmi

Get ipmi access

Returns ipmi credentials

### Example

```bash
 getdedicatedipmi id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getdedicatedos

Get dedicated server os

Returns operating system available

### Example

```bash
 getdedicatedos id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]

### Return type

[**array[OsDedie]**](OsDedie.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getdedicatedosrescue

Get dedicated os rescue

Returns dedicated os rescue

### Example

```bash
 getdedicatedosrescue id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getdedicatedplanaddons

Get dedicated server addons

Returns dedicated server addons available

### Example

```bash
 getdedicatedplanaddons id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | plan id | [default to null]

### Return type

[**array[OffreOptionDedie]**](OffreOptionDedie.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getdedicatedplanos

Get dedicated server os

Returns operating system available

### Example

```bash
 getdedicatedplanos id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | plan id | [default to null]

### Return type

[**array[OsDedie]**](OsDedie.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getdedicatedrescuecredentials

Get rescue credentials

Returns rescue credentials

### Example

```bash
 getdedicatedrescuecredentials id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getdedicatedserver

Get dedicated server informations

Returns dedicated server details

### Example

```bash
 getdedicatedserver id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | dedicated server id | [default to null]

### Return type

[**DedicatedServer**](DedicatedServer.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: object, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getdedicatedserverplan

Get dedicated server plans

Returns dedicated server plans

### Example

```bash
 getdedicatedserverplan
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**array[OffreDedie]**](OffreDedie.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getdedicatedservers

Get dedicated servers

Returns dedicated servers

### Example

```bash
 getdedicatedservers
```

### Parameters

This endpoint does not need any parameter.

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## postdedicatedboot

Post dedicated server boot normal mode

Set server normal boot mode

### Example

```bash
 postdedicatedboot id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## postdedicatedbootrescue

Post dedicated server rescue

Set server rescue mode

### Example

```bash
 postdedicatedbootrescue id=value  template=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]
 **template** | **string** | rescue template | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## postdedicatedhostname

Post dedicated server hostname

Set server hostname

### Example

```bash
 postdedicatedhostname id=value  hostname=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]
 **hostname** | **string** | server hostname | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## postdedicatedipmi

Create ipmi access

Request ipmi session

### Example

```bash
 postdedicatedipmi id=value  ip=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]
 **ip** | **string** | public ip | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## postdedicatedipreverse

Post ip reverse

Set IP reverse

### Example

```bash
 postdedicatedipreverse id=value  reverse=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]
 **reverse** | **string** | reverse | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## postdedicatedlabel

Post dedicated server label

Set dedicated server's label

### Example

```bash
 postdedicatedlabel id=value  label=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]
 **label** | **string** | label | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## postdedicatedreboot

Post dedicated server reboot

Returns reboot process

### Example

```bash
 postdedicatedreboot id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## postdedicatedserver

Create dedicated server

Order a new dedicated server

### Example

```bash
 postdedicatedserver  plan=value  os=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **plan** | **integer** | plan id | [default to null]
 **os** | **integer** | os id | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## postdedicatedsetup

Setup process

Starts setup process

### Example

```bash
 postdedicatedsetup id=value  os_id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]
 **osId** | **integer** | os id | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## postdedicatedshutdown

Post dedicated server shutdown

Returns shutdown process

### Example

```bash
 postdedicatedshutdown id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## terminatededicated

Terminate dedicated server

Terminate dedicated server

### Example

```bash
 terminatededicated id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | server id | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

