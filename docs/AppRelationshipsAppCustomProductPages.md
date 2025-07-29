# AppRelationshipsAppCustomProductPages


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppCustomProductPageVersionRelationshipsAppCustomProductPageData]**](AppCustomProductPageVersionRelationshipsAppCustomProductPageData.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_relationships_app_custom_product_pages import AppRelationshipsAppCustomProductPages

# TODO update the JSON string below
json = "{}"
# create an instance of AppRelationshipsAppCustomProductPages from a JSON string
app_relationships_app_custom_product_pages_instance = AppRelationshipsAppCustomProductPages.from_json(json)
# print the JSON string representation of the object
print(AppRelationshipsAppCustomProductPages.to_json())

# convert the object into a dict
app_relationships_app_custom_product_pages_dict = app_relationships_app_custom_product_pages_instance.to_dict()
# create an instance of AppRelationshipsAppCustomProductPages from a dict
app_relationships_app_custom_product_pages_from_dict = AppRelationshipsAppCustomProductPages.from_dict(app_relationships_app_custom_product_pages_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


