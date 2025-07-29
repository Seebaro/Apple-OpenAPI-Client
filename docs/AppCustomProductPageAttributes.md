# AppCustomProductPageAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**url** | **str** |  | [optional] 
**visible** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_attributes import AppCustomProductPageAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageAttributes from a JSON string
app_custom_product_page_attributes_instance = AppCustomProductPageAttributes.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageAttributes.to_json())

# convert the object into a dict
app_custom_product_page_attributes_dict = app_custom_product_page_attributes_instance.to_dict()
# create an instance of AppCustomProductPageAttributes from a dict
app_custom_product_page_attributes_from_dict = AppCustomProductPageAttributes.from_dict(app_custom_product_page_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


