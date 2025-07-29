# FileLocation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**path** | **str** |  | [optional] 
**line_number** | **int** |  | [optional] 

## Example

```python
from openapi_client.models.file_location import FileLocation

# TODO update the JSON string below
json = "{}"
# create an instance of FileLocation from a JSON string
file_location_instance = FileLocation.from_json(json)
# print the JSON string representation of the object
print(FileLocation.to_json())

# convert the object into a dict
file_location_dict = file_location_instance.to_dict()
# create an instance of FileLocation from a dict
file_location_from_dict = FileLocation.from_dict(file_location_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


