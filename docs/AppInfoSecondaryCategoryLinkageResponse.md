# AppInfoSecondaryCategoryLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppCategoryRelationshipsSubcategoriesDataInner**](AppCategoryRelationshipsSubcategoriesDataInner.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_info_secondary_category_linkage_response import AppInfoSecondaryCategoryLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppInfoSecondaryCategoryLinkageResponse from a JSON string
app_info_secondary_category_linkage_response_instance = AppInfoSecondaryCategoryLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppInfoSecondaryCategoryLinkageResponse.to_json())

# convert the object into a dict
app_info_secondary_category_linkage_response_dict = app_info_secondary_category_linkage_response_instance.to_dict()
# create an instance of AppInfoSecondaryCategoryLinkageResponse from a dict
app_info_secondary_category_linkage_response_from_dict = AppInfoSecondaryCategoryLinkageResponse.from_dict(app_info_secondary_category_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


