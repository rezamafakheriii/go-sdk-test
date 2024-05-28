# Connector

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Displayname** | Pointer to **string** |  | [optional] 
**Url** | Pointer to **string** |  | [optional] 

## Methods

### NewConnector

`func NewConnector() *Connector`

NewConnector instantiates a new Connector object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewConnectorWithDefaults

`func NewConnectorWithDefaults() *Connector`

NewConnectorWithDefaults instantiates a new Connector object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *Connector) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Connector) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Connector) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *Connector) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDisplayname

`func (o *Connector) GetDisplayname() string`

GetDisplayname returns the Displayname field if non-nil, zero value otherwise.

### GetDisplaynameOk

`func (o *Connector) GetDisplaynameOk() (*string, bool)`

GetDisplaynameOk returns a tuple with the Displayname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayname

`func (o *Connector) SetDisplayname(v string)`

SetDisplayname sets Displayname field to given value.

### HasDisplayname

`func (o *Connector) HasDisplayname() bool`

HasDisplayname returns a boolean if a field has been set.

### GetUrl

`func (o *Connector) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *Connector) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *Connector) SetUrl(v string)`

SetUrl sets Url field to given value.

### HasUrl

`func (o *Connector) HasUrl() bool`

HasUrl returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


