# BuildBundleFileSizeAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**device_model** | **str** |  | [optional] 
**os_version** | **str** |  | [optional] 
**download_bytes** | **int** |  | [optional] 
**install_bytes** | **int** |  | [optional] 

## Example

```python
from openapi_client.models.build_bundle_file_size_attributes import BuildBundleFileSizeAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of BuildBundleFileSizeAttributes from a JSON string
build_bundle_file_size_attributes_instance = BuildBundleFileSizeAttributes.from_json(json)
# print the JSON string representation of the object
print(BuildBundleFileSizeAttributes.to_json())

# convert the object into a dict
build_bundle_file_size_attributes_dict = build_bundle_file_size_attributes_instance.to_dict()
# create an instance of BuildBundleFileSizeAttributes from a dict
build_bundle_file_size_attributes_from_dict = BuildBundleFileSizeAttributes.from_dict(build_bundle_file_size_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


