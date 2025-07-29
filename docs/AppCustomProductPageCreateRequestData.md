# AppCustomProductPageCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppCustomProductPageCreateRequestDataAttributes**](AppCustomProductPageCreateRequestDataAttributes.md) |  | 
**relationships** | [**AppCustomProductPageCreateRequestDataRelationships**](AppCustomProductPageCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.app_custom_product_page_create_request_data import AppCustomProductPageCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageCreateRequestData from a JSON string
app_custom_product_page_create_request_data_instance = AppCustomProductPageCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageCreateRequestData.to_json())

# convert the object into a dict
app_custom_product_page_create_request_data_dict = app_custom_product_page_create_request_data_instance.to_dict()
# create an instance of AppCustomProductPageCreateRequestData from a dict
app_custom_product_page_create_request_data_from_dict = AppCustomProductPageCreateRequestData.from_dict(app_custom_product_page_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


