# BuildBetaBuildLocalizationsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BuildRelationshipsBetaBuildLocalizationsDataInner]**](BuildRelationshipsBetaBuildLocalizationsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.build_beta_build_localizations_linkages_response import BuildBetaBuildLocalizationsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BuildBetaBuildLocalizationsLinkagesResponse from a JSON string
build_beta_build_localizations_linkages_response_instance = BuildBetaBuildLocalizationsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(BuildBetaBuildLocalizationsLinkagesResponse.to_json())

# convert the object into a dict
build_beta_build_localizations_linkages_response_dict = build_beta_build_localizations_linkages_response_instance.to_dict()
# create an instance of BuildBetaBuildLocalizationsLinkagesResponse from a dict
build_beta_build_localizations_linkages_response_from_dict = BuildBetaBuildLocalizationsLinkagesResponse.from_dict(build_beta_build_localizations_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


