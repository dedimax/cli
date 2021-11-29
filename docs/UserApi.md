# UserApi

All URIs are relative to */api/3.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getnotifications**](UserApi.md#getnotifications) | **GET** /user/notifications | Get notifications
[**getuser**](UserApi.md#getuser) | **GET** /user | Get user informations
[**getwallet**](UserApi.md#getwallet) | **GET** /user/wallet | Get wallet informations



## getnotifications

Get notifications

Returns notifications data

### Example

```bash
 getnotifications
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**array[Notification]**](Notification.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getuser

Get user informations

Returns user informations

### Example

```bash
 getuser
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**User**](User.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: object, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## getwallet

Get wallet informations

Returns wallet data

### Example

```bash
 getwallet
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**Balance**](Balance.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

- **Content-Type**: Not Applicable
- **Accept**: object, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

