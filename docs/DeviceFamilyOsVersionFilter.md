# DeviceFamilyOsVersionFilter


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**device_family** | [**DeviceFamily**](DeviceFamily.md) |  | [optional] 
**minimum_os_inclusive** | **str** |  | [optional] 
**maximum_os_inclusive** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.device_family_os_version_filter import DeviceFamilyOsVersionFilter

# TODO update the JSON string below
json = "{}"
# create an instance of DeviceFamilyOsVersionFilter from a JSON string
device_family_os_version_filter_instance = DeviceFamilyOsVersionFilter.from_json(json)
# print the JSON string representation of the object
print(DeviceFamilyOsVersionFilter.to_json())

# convert the object into a dict
device_family_os_version_filter_dict = device_family_os_version_filter_instance.to_dict()
# create an instance of DeviceFamilyOsVersionFilter from a dict
device_family_os_version_filter_from_dict = DeviceFamilyOsVersionFilter.from_dict(device_family_os_version_filter_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


