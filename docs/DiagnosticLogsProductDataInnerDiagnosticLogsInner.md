# DiagnosticLogsProductDataInnerDiagnosticLogsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**call_stack_tree** | [**List[DiagnosticLogsProductDataInnerDiagnosticLogsInnerCallStackTreeInner]**](DiagnosticLogsProductDataInnerDiagnosticLogsInnerCallStackTreeInner.md) |  | [optional] 
**diagnostic_meta_data** | [**DiagnosticLogsProductDataInnerDiagnosticLogsInnerDiagnosticMetaData**](DiagnosticLogsProductDataInnerDiagnosticLogsInnerDiagnosticMetaData.md) |  | [optional] 

## Example

```python
from openapi_client.models.diagnostic_logs_product_data_inner_diagnostic_logs_inner import DiagnosticLogsProductDataInnerDiagnosticLogsInner

# TODO update the JSON string below
json = "{}"
# create an instance of DiagnosticLogsProductDataInnerDiagnosticLogsInner from a JSON string
diagnostic_logs_product_data_inner_diagnostic_logs_inner_instance = DiagnosticLogsProductDataInnerDiagnosticLogsInner.from_json(json)
# print the JSON string representation of the object
print(DiagnosticLogsProductDataInnerDiagnosticLogsInner.to_json())

# convert the object into a dict
diagnostic_logs_product_data_inner_diagnostic_logs_inner_dict = diagnostic_logs_product_data_inner_diagnostic_logs_inner_instance.to_dict()
# create an instance of DiagnosticLogsProductDataInnerDiagnosticLogsInner from a dict
diagnostic_logs_product_data_inner_diagnostic_logs_inner_from_dict = DiagnosticLogsProductDataInnerDiagnosticLogsInner.from_dict(diagnostic_logs_product_data_inner_diagnostic_logs_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


