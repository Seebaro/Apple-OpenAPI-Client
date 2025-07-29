# AppClipDomainStatusResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppClipDomainStatus**](AppClipDomainStatus.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_clip_domain_status_response import AppClipDomainStatusResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipDomainStatusResponse from a JSON string
app_clip_domain_status_response_instance = AppClipDomainStatusResponse.from_json(json)
# print the JSON string representation of the object
print(AppClipDomainStatusResponse.to_json())

# convert the object into a dict
app_clip_domain_status_response_dict = app_clip_domain_status_response_instance.to_dict()
# create an instance of AppClipDomainStatusResponse from a dict
app_clip_domain_status_response_from_dict = AppClipDomainStatusResponse.from_dict(app_clip_domain_status_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


