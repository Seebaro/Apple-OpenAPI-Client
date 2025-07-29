# BetaBuildLocalizationsWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BetaBuildLocalization]**](BetaBuildLocalization.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_build_localizations_without_includes_response import BetaBuildLocalizationsWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaBuildLocalizationsWithoutIncludesResponse from a JSON string
beta_build_localizations_without_includes_response_instance = BetaBuildLocalizationsWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(BetaBuildLocalizationsWithoutIncludesResponse.to_json())

# convert the object into a dict
beta_build_localizations_without_includes_response_dict = beta_build_localizations_without_includes_response_instance.to_dict()
# create an instance of BetaBuildLocalizationsWithoutIncludesResponse from a dict
beta_build_localizations_without_includes_response_from_dict = BetaBuildLocalizationsWithoutIncludesResponse.from_dict(beta_build_localizations_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


