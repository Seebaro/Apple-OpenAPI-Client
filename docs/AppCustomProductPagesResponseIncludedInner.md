# AppCustomProductPagesResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppCustomProductPageVersionAttributes**](AppCustomProductPageVersionAttributes.md) |  | [optional] 
**relationships** | [**AppCustomProductPageVersionRelationships**](AppCustomProductPageVersionRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_pages_response_included_inner import AppCustomProductPagesResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPagesResponseIncludedInner from a JSON string
app_custom_product_pages_response_included_inner_instance = AppCustomProductPagesResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPagesResponseIncludedInner.to_json())

# convert the object into a dict
app_custom_product_pages_response_included_inner_dict = app_custom_product_pages_response_included_inner_instance.to_dict()
# create an instance of AppCustomProductPagesResponseIncludedInner from a dict
app_custom_product_pages_response_included_inner_from_dict = AppCustomProductPagesResponseIncludedInner.from_dict(app_custom_product_pages_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


