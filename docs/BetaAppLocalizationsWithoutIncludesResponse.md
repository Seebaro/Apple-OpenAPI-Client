# BetaAppLocalizationsWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BetaAppLocalization]**](BetaAppLocalization.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_app_localizations_without_includes_response import BetaAppLocalizationsWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaAppLocalizationsWithoutIncludesResponse from a JSON string
beta_app_localizations_without_includes_response_instance = BetaAppLocalizationsWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(BetaAppLocalizationsWithoutIncludesResponse.to_json())

# convert the object into a dict
beta_app_localizations_without_includes_response_dict = beta_app_localizations_without_includes_response_instance.to_dict()
# create an instance of BetaAppLocalizationsWithoutIncludesResponse from a dict
beta_app_localizations_without_includes_response_from_dict = BetaAppLocalizationsWithoutIncludesResponse.from_dict(beta_app_localizations_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


