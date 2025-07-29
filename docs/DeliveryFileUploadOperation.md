# DeliveryFileUploadOperation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**method** | **str** |  | [optional] 
**url** | **str** |  | [optional] 
**length** | **int** |  | [optional] 
**offset** | **int** |  | [optional] 
**request_headers** | [**List[HttpHeader]**](HttpHeader.md) |  | [optional] 
**expiration** | **datetime** |  | [optional] 
**part_number** | **int** |  | [optional] 
**entity_tag** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.delivery_file_upload_operation import DeliveryFileUploadOperation

# TODO update the JSON string below
json = "{}"
# create an instance of DeliveryFileUploadOperation from a JSON string
delivery_file_upload_operation_instance = DeliveryFileUploadOperation.from_json(json)
# print the JSON string representation of the object
print(DeliveryFileUploadOperation.to_json())

# convert the object into a dict
delivery_file_upload_operation_dict = delivery_file_upload_operation_instance.to_dict()
# create an instance of DeliveryFileUploadOperation from a dict
delivery_file_upload_operation_from_dict = DeliveryFileUploadOperation.from_dict(delivery_file_upload_operation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


