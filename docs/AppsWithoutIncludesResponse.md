# AppsWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[App]**](App.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.apps_without_includes_response import AppsWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppsWithoutIncludesResponse from a JSON string
apps_without_includes_response_instance = AppsWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(AppsWithoutIncludesResponse.to_json())

# convert the object into a dict
apps_without_includes_response_dict = apps_without_includes_response_instance.to_dict()
# create an instance of AppsWithoutIncludesResponse from a dict
apps_without_includes_response_from_dict = AppsWithoutIncludesResponse.from_dict(apps_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


