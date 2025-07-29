# AppInfoPrimaryCategoryLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppCategoryRelationshipsSubcategoriesDataInner**](AppCategoryRelationshipsSubcategoriesDataInner.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_info_primary_category_linkage_response import AppInfoPrimaryCategoryLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppInfoPrimaryCategoryLinkageResponse from a JSON string
app_info_primary_category_linkage_response_instance = AppInfoPrimaryCategoryLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppInfoPrimaryCategoryLinkageResponse.to_json())

# convert the object into a dict
app_info_primary_category_linkage_response_dict = app_info_primary_category_linkage_response_instance.to_dict()
# create an instance of AppInfoPrimaryCategoryLinkageResponse from a dict
app_info_primary_category_linkage_response_from_dict = AppInfoPrimaryCategoryLinkageResponse.from_dict(app_info_primary_category_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


