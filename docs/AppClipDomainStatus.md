# AppClipDomainStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipDomainStatusAttributes**](AppClipDomainStatusAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_domain_status import AppClipDomainStatus

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipDomainStatus from a JSON string
app_clip_domain_status_instance = AppClipDomainStatus.from_json(json)
# print the JSON string representation of the object
print(AppClipDomainStatus.to_json())

# convert the object into a dict
app_clip_domain_status_dict = app_clip_domain_status_instance.to_dict()
# create an instance of AppClipDomainStatus from a dict
app_clip_domain_status_from_dict = AppClipDomainStatus.from_dict(app_clip_domain_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


