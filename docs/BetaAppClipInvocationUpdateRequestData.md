# BetaAppClipInvocationUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BetaAppClipInvocationAttributes**](BetaAppClipInvocationAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_app_clip_invocation_update_request_data import BetaAppClipInvocationUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of BetaAppClipInvocationUpdateRequestData from a JSON string
beta_app_clip_invocation_update_request_data_instance = BetaAppClipInvocationUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(BetaAppClipInvocationUpdateRequestData.to_json())

# convert the object into a dict
beta_app_clip_invocation_update_request_data_dict = beta_app_clip_invocation_update_request_data_instance.to_dict()
# create an instance of BetaAppClipInvocationUpdateRequestData from a dict
beta_app_clip_invocation_update_request_data_from_dict = BetaAppClipInvocationUpdateRequestData.from_dict(beta_app_clip_invocation_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


