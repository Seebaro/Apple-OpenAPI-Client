# BuildBundleFileSizesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BuildBundleFileSize]**](BuildBundleFileSize.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.build_bundle_file_sizes_response import BuildBundleFileSizesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BuildBundleFileSizesResponse from a JSON string
build_bundle_file_sizes_response_instance = BuildBundleFileSizesResponse.from_json(json)
# print the JSON string representation of the object
print(BuildBundleFileSizesResponse.to_json())

# convert the object into a dict
build_bundle_file_sizes_response_dict = build_bundle_file_sizes_response_instance.to_dict()
# create an instance of BuildBundleFileSizesResponse from a dict
build_bundle_file_sizes_response_from_dict = BuildBundleFileSizesResponse.from_dict(build_bundle_file_sizes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


