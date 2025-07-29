# ProfileDevicesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[ProfileRelationshipsDevicesDataInner]**](ProfileRelationshipsDevicesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.profile_devices_linkages_response import ProfileDevicesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ProfileDevicesLinkagesResponse from a JSON string
profile_devices_linkages_response_instance = ProfileDevicesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(ProfileDevicesLinkagesResponse.to_json())

# convert the object into a dict
profile_devices_linkages_response_dict = profile_devices_linkages_response_instance.to_dict()
# create an instance of ProfileDevicesLinkagesResponse from a dict
profile_devices_linkages_response_from_dict = ProfileDevicesLinkagesResponse.from_dict(profile_devices_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


