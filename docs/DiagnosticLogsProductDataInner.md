# DiagnosticLogsProductDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**signature_id** | **str** |  | [optional] 
**diagnostic_insights** | [**List[DiagnosticLogsProductDataInnerDiagnosticInsightsInner]**](DiagnosticLogsProductDataInnerDiagnosticInsightsInner.md) |  | [optional] 
**diagnostic_logs** | [**List[DiagnosticLogsProductDataInnerDiagnosticLogsInner]**](DiagnosticLogsProductDataInnerDiagnosticLogsInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.diagnostic_logs_product_data_inner import DiagnosticLogsProductDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of DiagnosticLogsProductDataInner from a JSON string
diagnostic_logs_product_data_inner_instance = DiagnosticLogsProductDataInner.from_json(json)
# print the JSON string representation of the object
print(DiagnosticLogsProductDataInner.to_json())

# convert the object into a dict
diagnostic_logs_product_data_inner_dict = diagnostic_logs_product_data_inner_instance.to_dict()
# create an instance of DiagnosticLogsProductDataInner from a dict
diagnostic_logs_product_data_inner_from_dict = DiagnosticLogsProductDataInner.from_dict(diagnostic_logs_product_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


