# BetaBuildLocalizationBuildLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppEncryptionDeclarationRelationshipsBuildsDataInner**](AppEncryptionDeclarationRelationshipsBuildsDataInner.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.beta_build_localization_build_linkage_response import BetaBuildLocalizationBuildLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaBuildLocalizationBuildLinkageResponse from a JSON string
beta_build_localization_build_linkage_response_instance = BetaBuildLocalizationBuildLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(BetaBuildLocalizationBuildLinkageResponse.to_json())

# convert the object into a dict
beta_build_localization_build_linkage_response_dict = beta_build_localization_build_linkage_response_instance.to_dict()
# create an instance of BetaBuildLocalizationBuildLinkageResponse from a dict
beta_build_localization_build_linkage_response_from_dict = BetaBuildLocalizationBuildLinkageResponse.from_dict(beta_build_localization_build_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


