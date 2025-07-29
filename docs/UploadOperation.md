# UploadOperation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**method** | **str** |  | [optional] 
**url** | **str** |  | [optional] 
**length** | **int** |  | [optional] 
**offset** | **int** |  | [optional] 
**request_headers** | [**List[HttpHeader]**](HttpHeader.md) |  | [optional] 

## Example

```python
from openapi_client.models.upload_operation import UploadOperation

# TODO update the JSON string below
json = "{}"
# create an instance of UploadOperation from a JSON string
upload_operation_instance = UploadOperation.from_json(json)
# print the JSON string representation of the object
print(UploadOperation.to_json())

# convert the object into a dict
upload_operation_dict = upload_operation_instance.to_dict()
# create an instance of UploadOperation from a dict
upload_operation_from_dict = UploadOperation.from_dict(upload_operation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


