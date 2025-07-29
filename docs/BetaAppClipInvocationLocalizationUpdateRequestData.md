# BetaAppClipInvocationLocalizationUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BetaAppClipInvocationLocalizationUpdateRequestDataAttributes**](BetaAppClipInvocationLocalizationUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_app_clip_invocation_localization_update_request_data import BetaAppClipInvocationLocalizationUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of BetaAppClipInvocationLocalizationUpdateRequestData from a JSON string
beta_app_clip_invocation_localization_update_request_data_instance = BetaAppClipInvocationLocalizationUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(BetaAppClipInvocationLocalizationUpdateRequestData.to_json())

# convert the object into a dict
beta_app_clip_invocation_localization_update_request_data_dict = beta_app_clip_invocation_localization_update_request_data_instance.to_dict()
# create an instance of BetaAppClipInvocationLocalizationUpdateRequestData from a dict
beta_app_clip_invocation_localization_update_request_data_from_dict = BetaAppClipInvocationLocalizationUpdateRequestData.from_dict(beta_app_clip_invocation_localization_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


