# AnalyticsReportRequestResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AnalyticsReportRequest**](AnalyticsReportRequest.md) |  | 
**included** | [**List[AnalyticsReport]**](AnalyticsReport.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.analytics_report_request_response import AnalyticsReportRequestResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportRequestResponse from a JSON string
analytics_report_request_response_instance = AnalyticsReportRequestResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportRequestResponse.to_json())

# convert the object into a dict
analytics_report_request_response_dict = analytics_report_request_response_instance.to_dict()
# create an instance of AnalyticsReportRequestResponse from a dict
analytics_report_request_response_from_dict = AnalyticsReportRequestResponse.from_dict(analytics_report_request_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


