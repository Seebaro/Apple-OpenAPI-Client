# DiagnosticLogs


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**product_data** | [**List[DiagnosticLogsProductDataInner]**](DiagnosticLogsProductDataInner.md) |  | [optional] 
**version** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.diagnostic_logs import DiagnosticLogs

# TODO update the JSON string below
json = "{}"
# create an instance of DiagnosticLogs from a JSON string
diagnostic_logs_instance = DiagnosticLogs.from_json(json)
# print the JSON string representation of the object
print(DiagnosticLogs.to_json())

# convert the object into a dict
diagnostic_logs_dict = diagnostic_logs_instance.to_dict()
# create an instance of DiagnosticLogs from a dict
diagnostic_logs_from_dict = DiagnosticLogs.from_dict(diagnostic_logs_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


