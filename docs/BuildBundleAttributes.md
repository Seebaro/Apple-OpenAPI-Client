# BuildBundleAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bundle_id** | **str** |  | [optional] 
**bundle_type** | [**BuildBundleType**](BuildBundleType.md) |  | [optional] 
**sdk_build** | **str** |  | [optional] 
**platform_build** | **str** |  | [optional] 
**file_name** | **str** |  | [optional] 
**has_sirikit** | **bool** |  | [optional] 
**has_on_demand_resources** | **bool** |  | [optional] 
**has_prerendered_icon** | **bool** |  | [optional] 
**uses_location_services** | **bool** |  | [optional] 
**is_ios_build_mac_app_store_compatible** | **bool** |  | [optional] 
**includes_symbols** | **bool** |  | [optional] 
**d_sym_url** | **str** |  | [optional] 
**supported_architectures** | **List[str]** |  | [optional] 
**required_capabilities** | **List[str]** |  | [optional] 
**device_protocols** | **List[str]** |  | [optional] 
**locales** | **List[str]** |  | [optional] 
**entitlements** | **Dict[str, Dict[str, str]]** |  | [optional] 
**ba_download_allowance** | **int** |  | [optional] 
**ba_max_install_size** | **int** |  | [optional] 

## Example

```python
from openapi_client.models.build_bundle_attributes import BuildBundleAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of BuildBundleAttributes from a JSON string
build_bundle_attributes_instance = BuildBundleAttributes.from_json(json)
# print the JSON string representation of the object
print(BuildBundleAttributes.to_json())

# convert the object into a dict
build_bundle_attributes_dict = build_bundle_attributes_instance.to_dict()
# create an instance of BuildBundleAttributes from a dict
build_bundle_attributes_from_dict = BuildBundleAttributes.from_dict(build_bundle_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


