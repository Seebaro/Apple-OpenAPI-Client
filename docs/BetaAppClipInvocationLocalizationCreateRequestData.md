# BetaAppClipInvocationLocalizationCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**BetaAppClipInvocationLocalizationInlineCreateAttributes**](BetaAppClipInvocationLocalizationInlineCreateAttributes.md) |  | 
**relationships** | [**BetaAppClipInvocationLocalizationCreateRequestDataRelationships**](BetaAppClipInvocationLocalizationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.beta_app_clip_invocation_localization_create_request_data import BetaAppClipInvocationLocalizationCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of BetaAppClipInvocationLocalizationCreateRequestData from a JSON string
beta_app_clip_invocation_localization_create_request_data_instance = BetaAppClipInvocationLocalizationCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(BetaAppClipInvocationLocalizationCreateRequestData.to_json())

# convert the object into a dict
beta_app_clip_invocation_localization_create_request_data_dict = beta_app_clip_invocation_localization_create_request_data_instance.to_dict()
# create an instance of BetaAppClipInvocationLocalizationCreateRequestData from a dict
beta_app_clip_invocation_localization_create_request_data_from_dict = BetaAppClipInvocationLocalizationCreateRequestData.from_dict(beta_app_clip_invocation_localization_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


