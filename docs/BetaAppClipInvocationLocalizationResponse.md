# BetaAppClipInvocationLocalizationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BetaAppClipInvocationLocalization**](BetaAppClipInvocationLocalization.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.beta_app_clip_invocation_localization_response import BetaAppClipInvocationLocalizationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaAppClipInvocationLocalizationResponse from a JSON string
beta_app_clip_invocation_localization_response_instance = BetaAppClipInvocationLocalizationResponse.from_json(json)
# print the JSON string representation of the object
print(BetaAppClipInvocationLocalizationResponse.to_json())

# convert the object into a dict
beta_app_clip_invocation_localization_response_dict = beta_app_clip_invocation_localization_response_instance.to_dict()
# create an instance of BetaAppClipInvocationLocalizationResponse from a dict
beta_app_clip_invocation_localization_response_from_dict = BetaAppClipInvocationLocalizationResponse.from_dict(beta_app_clip_invocation_localization_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


