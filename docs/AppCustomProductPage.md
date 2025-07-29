# AppCustomProductPage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppCustomProductPageAttributes**](AppCustomProductPageAttributes.md) |  | [optional] 
**relationships** | [**AppCustomProductPageRelationships**](AppCustomProductPageRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page import AppCustomProductPage

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPage from a JSON string
app_custom_product_page_instance = AppCustomProductPage.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPage.to_json())

# convert the object into a dict
app_custom_product_page_dict = app_custom_product_page_instance.to_dict()
# create an instance of AppCustomProductPage from a dict
app_custom_product_page_from_dict = AppCustomProductPage.from_dict(app_custom_product_page_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


