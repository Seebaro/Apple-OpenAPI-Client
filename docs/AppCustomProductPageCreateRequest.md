# AppCustomProductPageCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppCustomProductPageCreateRequestData**](AppCustomProductPageCreateRequestData.md) |  | 
**included** | [**List[AppCustomProductPageCreateRequestIncludedInner]**](AppCustomProductPageCreateRequestIncludedInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_create_request import AppCustomProductPageCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageCreateRequest from a JSON string
app_custom_product_page_create_request_instance = AppCustomProductPageCreateRequest.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageCreateRequest.to_json())

# convert the object into a dict
app_custom_product_page_create_request_dict = app_custom_product_page_create_request_instance.to_dict()
# create an instance of AppCustomProductPageCreateRequest from a dict
app_custom_product_page_create_request_from_dict = AppCustomProductPageCreateRequest.from_dict(app_custom_product_page_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


