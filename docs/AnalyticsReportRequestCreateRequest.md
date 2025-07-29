# AnalyticsReportRequestCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AnalyticsReportRequestCreateRequestData**](AnalyticsReportRequestCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.analytics_report_request_create_request import AnalyticsReportRequestCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportRequestCreateRequest from a JSON string
analytics_report_request_create_request_instance = AnalyticsReportRequestCreateRequest.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportRequestCreateRequest.to_json())

# convert the object into a dict
analytics_report_request_create_request_dict = analytics_report_request_create_request_instance.to_dict()
# create an instance of AnalyticsReportRequestCreateRequest from a dict
analytics_report_request_create_request_from_dict = AnalyticsReportRequestCreateRequest.from_dict(analytics_report_request_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


