# AppInfoAgeRatingDeclarationLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppInfoRelationshipsAgeRatingDeclarationData**](AppInfoRelationshipsAgeRatingDeclarationData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_info_age_rating_declaration_linkage_response import AppInfoAgeRatingDeclarationLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppInfoAgeRatingDeclarationLinkageResponse from a JSON string
app_info_age_rating_declaration_linkage_response_instance = AppInfoAgeRatingDeclarationLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppInfoAgeRatingDeclarationLinkageResponse.to_json())

# convert the object into a dict
app_info_age_rating_declaration_linkage_response_dict = app_info_age_rating_declaration_linkage_response_instance.to_dict()
# create an instance of AppInfoAgeRatingDeclarationLinkageResponse from a dict
app_info_age_rating_declaration_linkage_response_from_dict = AppInfoAgeRatingDeclarationLinkageResponse.from_dict(app_info_age_rating_declaration_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


