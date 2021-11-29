# CloudApi

All URIs are relative to */api/3.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cloudterminate**](CloudApi.md#cloudterminate) | **DELETE** /cloud/{id} | Terminate cloud server
[**getcloud**](CloudApi.md#getcloud) | **GET** /cloud/{id} | Get cloud informations
[**getcloudaddons**](CloudApi.md#getcloudaddons) | **GET** /cloud/addons | Get cloud addons
[**getcloudipdetails**](CloudApi.md#getcloudipdetails) | **GET** /cloud/{id}/ips/{ip} | Get cloud ip details
[**getcloudips**](CloudApi.md#getcloudips) | **GET** /cloud/{id}/ips | Get cloud ips
[**getcloudlocation**](CloudApi.md#getcloudlocation) | **GET** /cloud/location | Get cloud locations
[**getcloudplan**](CloudApi.md#getcloudplan) | **GET** /cloud/plan | Get cloud plans
[**getcloudreboot**](CloudApi.md#getcloudreboot) | **GET** /cloud/{id}/reboot | Get cloud reboot
[**getclouds**](CloudApi.md#getclouds) | **GET** /cloud | Get cloud servers
[**getcloudshutdown**](CloudApi.md#getcloudshutdown) | **GET** /cloud/{id}/shutdown | Get cloud shutdown
[**getcloudtemplates**](CloudApi.md#getcloudtemplates) | **GET** /cloud/templates | Get cloud templates
[**postcloud**](CloudApi.md#postcloud) | **POST** /cloud | Create new cloud server
[**postcloudclone**](CloudApi.md#postcloudclone) | **POST** /cloud/{id}/clone | Post cloud clone
[**postcloudhostname**](CloudApi.md#postcloudhostname) | **POST** /cloud/{id}/hostname | Post cloud hostname
[**postcloudlabel**](CloudApi.md#postcloudlabel) | **POST** /cloud/{id}/label | Post cloud label
[**postcloudupgrade**](CloudApi.md#postcloudupgrade) | **POST** /cloud/{id}/upgrade | Upgrade cloud server
[**setcloudipreverse**](CloudApi.md#setcloudipreverse) | **POST** /cloud/{id}/ips/{ip}/reverse | Post cloud ip reverse
[**setcloudsetup**](CloudApi.md#setcloudsetup) | **POST** /cloud/{id}/setup | Post cloud setup



## cloudterminate

Terminate cloud server

Terminate cloud server

### Example

```bash
 cloudterminate id=value
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


## getcloud

Get cloud informations

Returns cloud data

### Example

```bash
 getcloud id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | cloud id | [default to null]

### Return type

[**Cloud**](Cloud.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: object, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getcloudaddons

Get cloud addons

Returns cloud addons

### Example

```bash
 getcloudaddons
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**array[OffreOptionCloud]**](OffreOptionCloud.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getcloudipdetails

Get cloud ip details

Returns cloud ip details

### Example

```bash
 getcloudipdetails id=value ip=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | cloud id | [default to null]
 **ip** | **string** | cloud ip | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getcloudips

Get cloud ips

Returns cloud ips

### Example

```bash
 getcloudips id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | cloud id | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getcloudlocation

Get cloud locations

Returns cloud locations

### Example

```bash
 getcloudlocation
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**CloudLocation**](CloudLocation.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: json, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getcloudplan

Get cloud plans

Returns cloud plans

### Example

```bash
 getcloudplan
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**array[OffreCloud]**](OffreCloud.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getcloudreboot

Get cloud reboot

cloud reboot

### Example

```bash
 getcloudreboot id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | cloud id | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getclouds

Get cloud servers

Returns cloud servers

### Example

```bash
 getclouds
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


## getcloudshutdown

Get cloud shutdown

cloud shutdown

### Example

```bash
 getcloudshutdown id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | cloud id | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getcloudtemplates

Get cloud templates

Returns cloud templates

### Example

```bash
 getcloudtemplates
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**array[OsCloud]**](OsCloud.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## postcloud

Create new cloud server

Deploy a new cloud server

### Example

```bash
 postcloud  plan=value  location=value  os=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **plan** | **integer** | plan id (/cloud/plan method) | [default to null]
 **location** | **integer** | location id (/cloud/location method) | [default to null]
 **os** | **integer** | template id (/cloud/templates method) | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## postcloudclone

Post cloud clone

cloud clone

### Example

```bash
 postcloudclone id=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | cloud id | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## postcloudhostname

Post cloud hostname

Set cloud hostname

### Example

```bash
 postcloudhostname id=value  hostname=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | cloud id | [default to null]
 **hostname** | **string** | cloud hostname | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## postcloudlabel

Post cloud label

Set cloud label

### Example

```bash
 postcloudlabel id=value  label=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | cloud id | [default to null]
 **label** | **string** | cloud label | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## postcloudupgrade

Upgrade cloud server

Upgrade cloud server

### Example

```bash
 postcloudupgrade id=value  plan=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | cloud id | [default to null]
 **plan** | **string** | cloud plan | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## setcloudipreverse

Post cloud ip reverse

Set cloud ip reverse

### Example

```bash
 setcloudipreverse id=value ip=value  reverse=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | cloud id | [default to null]
 **ip** | **integer** | cloud ip | [default to null]
 **reverse** | **string** | reverse | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## setcloudsetup

Post cloud setup

cloud setup

### Example

```bash
 setcloudsetup id=value  template=value
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **integer** | cloud id | [default to null]
 **template** | **integer** | template id | [default to null]

### Return type

(empty response body)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

