# AnalyticsReportInstanceResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AnalyticsReportInstance**](AnalyticsReportInstance.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.analytics_report_instance_response import AnalyticsReportInstanceResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportInstanceResponse from a JSON string
analytics_report_instance_response_instance = AnalyticsReportInstanceResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportInstanceResponse.to_json())

# convert the object into a dict
analytics_report_instance_response_dict = analytics_report_instance_response_instance.to_dict()
# create an instance of AnalyticsReportInstanceResponse from a dict
analytics_report_instance_response_from_dict = AnalyticsReportInstanceResponse.from_dict(analytics_report_instance_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


