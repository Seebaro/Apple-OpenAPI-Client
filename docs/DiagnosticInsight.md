# DiagnosticInsight


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**insight_type** | [**DiagnosticInsightType**](DiagnosticInsightType.md) |  | [optional] 
**direction** | [**DiagnosticInsightDirection**](DiagnosticInsightDirection.md) |  | [optional] 
**reference_versions** | [**List[DiagnosticInsightReferenceVersionsInner]**](DiagnosticInsightReferenceVersionsInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.diagnostic_insight import DiagnosticInsight

# TODO update the JSON string below
json = "{}"
# create an instance of DiagnosticInsight from a JSON string
diagnostic_insight_instance = DiagnosticInsight.from_json(json)
# print the JSON string representation of the object
print(DiagnosticInsight.to_json())

# convert the object into a dict
diagnostic_insight_dict = diagnostic_insight_instance.to_dict()
# create an instance of DiagnosticInsight from a dict
diagnostic_insight_from_dict = DiagnosticInsight.from_dict(diagnostic_insight_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


