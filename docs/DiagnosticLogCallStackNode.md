# DiagnosticLogCallStackNode


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sample_count** | **int** |  | [optional] 
**is_blame_frame** | **bool** |  | [optional] 
**symbol_name** | **str** |  | [optional] 
**insights_category** | **str** |  | [optional] 
**offset_into_symbol** | **str** |  | [optional] 
**binary_name** | **str** |  | [optional] 
**file_name** | **str** |  | [optional] 
**binary_uuid** | **str** |  | [optional] 
**line_number** | **str** |  | [optional] 
**address** | **str** |  | [optional] 
**offset_into_binary_text_segment** | **str** |  | [optional] 
**raw_frame** | **str** |  | [optional] 
**sub_frames** | [**List[DiagnosticLogCallStackNode]**](DiagnosticLogCallStackNode.md) |  | [optional] 

## Example

```python
from openapi_client.models.diagnostic_log_call_stack_node import DiagnosticLogCallStackNode

# TODO update the JSON string below
json = "{}"
# create an instance of DiagnosticLogCallStackNode from a JSON string
diagnostic_log_call_stack_node_instance = DiagnosticLogCallStackNode.from_json(json)
# print the JSON string representation of the object
print(DiagnosticLogCallStackNode.to_json())

# convert the object into a dict
diagnostic_log_call_stack_node_dict = diagnostic_log_call_stack_node_instance.to_dict()
# create an instance of DiagnosticLogCallStackNode from a dict
diagnostic_log_call_stack_node_from_dict = DiagnosticLogCallStackNode.from_dict(diagnostic_log_call_stack_node_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


