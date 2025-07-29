# BundleIdWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BundleId**](BundleId.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.bundle_id_without_includes_response import BundleIdWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BundleIdWithoutIncludesResponse from a JSON string
bundle_id_without_includes_response_instance = BundleIdWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(BundleIdWithoutIncludesResponse.to_json())

# convert the object into a dict
bundle_id_without_includes_response_dict = bundle_id_without_includes_response_instance.to_dict()
# create an instance of BundleIdWithoutIncludesResponse from a dict
bundle_id_without_includes_response_from_dict = BundleIdWithoutIncludesResponse.from_dict(bundle_id_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


