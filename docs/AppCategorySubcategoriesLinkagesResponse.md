# AppCategorySubcategoriesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppCategoryRelationshipsSubcategoriesDataInner]**](AppCategoryRelationshipsSubcategoriesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_category_subcategories_linkages_response import AppCategorySubcategoriesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppCategorySubcategoriesLinkagesResponse from a JSON string
app_category_subcategories_linkages_response_instance = AppCategorySubcategoriesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppCategorySubcategoriesLinkagesResponse.to_json())

# convert the object into a dict
app_category_subcategories_linkages_response_dict = app_category_subcategories_linkages_response_instance.to_dict()
# create an instance of AppCategorySubcategoriesLinkagesResponse from a dict
app_category_subcategories_linkages_response_from_dict = AppCategorySubcategoriesLinkagesResponse.from_dict(app_category_subcategories_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


