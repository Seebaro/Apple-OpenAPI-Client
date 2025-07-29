# AnalyticsReportResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AnalyticsReport**](AnalyticsReport.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.analytics_report_response import AnalyticsReportResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportResponse from a JSON string
analytics_report_response_instance = AnalyticsReportResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportResponse.to_json())

# convert the object into a dict
analytics_report_response_dict = analytics_report_response_instance.to_dict()
# create an instance of AnalyticsReportResponse from a dict
analytics_report_response_from_dict = AnalyticsReportResponse.from_dict(analytics_report_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


