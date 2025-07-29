# BetaAppClipInvocationLocalization


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BetaAppClipInvocationLocalizationAttributes**](BetaAppClipInvocationLocalizationAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_app_clip_invocation_localization import BetaAppClipInvocationLocalization

# TODO update the JSON string below
json = "{}"
# create an instance of BetaAppClipInvocationLocalization from a JSON string
beta_app_clip_invocation_localization_instance = BetaAppClipInvocationLocalization.from_json(json)
# print the JSON string representation of the object
print(BetaAppClipInvocationLocalization.to_json())

# convert the object into a dict
beta_app_clip_invocation_localization_dict = beta_app_clip_invocation_localization_instance.to_dict()
# create an instance of BetaAppClipInvocationLocalization from a dict
beta_app_clip_invocation_localization_from_dict = BetaAppClipInvocationLocalization.from_dict(beta_app_clip_invocation_localization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


