# \GophersAPI

All URIs are relative to *http://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ConnectorDelete**](GophersAPI.md#ConnectorDelete) | **Delete** /connector | 
[**ConnectorGet**](GophersAPI.md#ConnectorGet) | **Get** /connector | 
[**ConnectorPost**](GophersAPI.md#ConnectorPost) | **Post** /connector | Add a new Connector
[**ConnectorPut**](GophersAPI.md#ConnectorPut) | **Put** /connector | 



## ConnectorDelete

> ConnectorDelete(ctx).Name(name).Execute()





### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rezamafakheriii/go-sdk-test"
)

func main() {
	name := "name_example" // string | Connector name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.GophersAPI.ConnectorDelete(context.Background()).Name(name).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GophersAPI.ConnectorDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiConnectorDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **string** | Connector name | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ConnectorGet

> Connector ConnectorGet(ctx).Name(name).Execute()





### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rezamafakheriii/go-sdk-test"
)

func main() {
	name := "name_example" // string | Connector name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GophersAPI.ConnectorGet(context.Background()).Name(name).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GophersAPI.ConnectorGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ConnectorGet`: Connector
	fmt.Fprintf(os.Stdout, "Response from `GophersAPI.ConnectorGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiConnectorGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **string** | Connector name | 

### Return type

[**Connector**](Connector.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ConnectorPost

> Connector ConnectorPost(ctx).Connector(connector).Execute()

Add a new Connector

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rezamafakheriii/go-sdk-test"
)

func main() {
	connector := *openapiclient.NewConnectorPutRequest("Name_example", "Displayname_example", "Url_example") // ConnectorPutRequest | The Connector to create. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GophersAPI.ConnectorPost(context.Background()).Connector(connector).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GophersAPI.ConnectorPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ConnectorPost`: Connector
	fmt.Fprintf(os.Stdout, "Response from `GophersAPI.ConnectorPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiConnectorPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connector** | [**ConnectorPutRequest**](ConnectorPutRequest.md) | The Connector to create. | 

### Return type

[**Connector**](Connector.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ConnectorPut

> Connector ConnectorPut(ctx).Connector(connector).Execute()





### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/rezamafakheriii/go-sdk-test"
)

func main() {
	connector := *openapiclient.NewConnectorPutRequest("Name_example", "Displayname_example", "Url_example") // ConnectorPutRequest | The Connector to update. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GophersAPI.ConnectorPut(context.Background()).Connector(connector).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GophersAPI.ConnectorPut``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ConnectorPut`: Connector
	fmt.Fprintf(os.Stdout, "Response from `GophersAPI.ConnectorPut`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiConnectorPutRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connector** | [**ConnectorPutRequest**](ConnectorPutRequest.md) | The Connector to update. | 

### Return type

[**Connector**](Connector.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

