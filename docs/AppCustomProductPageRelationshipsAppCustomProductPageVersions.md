# AppCustomProductPageRelationshipsAppCustomProductPageVersions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppCustomProductPageLocalizationRelationshipsAppCustomProductPageVersionData]**](AppCustomProductPageLocalizationRelationshipsAppCustomProductPageVersionData.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_relationships_app_custom_product_page_versions import AppCustomProductPageRelationshipsAppCustomProductPageVersions

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageRelationshipsAppCustomProductPageVersions from a JSON string
app_custom_product_page_relationships_app_custom_product_page_versions_instance = AppCustomProductPageRelationshipsAppCustomProductPageVersions.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageRelationshipsAppCustomProductPageVersions.to_json())

# convert the object into a dict
app_custom_product_page_relationships_app_custom_product_page_versions_dict = app_custom_product_page_relationships_app_custom_product_page_versions_instance.to_dict()
# create an instance of AppCustomProductPageRelationshipsAppCustomProductPageVersions from a dict
app_custom_product_page_relationships_app_custom_product_page_versions_from_dict = AppCustomProductPageRelationshipsAppCustomProductPageVersions.from_dict(app_custom_product_page_relationships_app_custom_product_page_versions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


