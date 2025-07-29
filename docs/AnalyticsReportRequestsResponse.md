# AnalyticsReportRequestsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AnalyticsReportRequest]**](AnalyticsReportRequest.md) |  | 
**included** | [**List[AnalyticsReport]**](AnalyticsReport.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.analytics_report_requests_response import AnalyticsReportRequestsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportRequestsResponse from a JSON string
analytics_report_requests_response_instance = AnalyticsReportRequestsResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportRequestsResponse.to_json())

# convert the object into a dict
analytics_report_requests_response_dict = analytics_report_requests_response_instance.to_dict()
# create an instance of AnalyticsReportRequestsResponse from a dict
analytics_report_requests_response_from_dict = AnalyticsReportRequestsResponse.from_dict(analytics_report_requests_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


