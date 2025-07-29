# AppAnalyticsReportRequestsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppAnalyticsReportRequestsLinkagesResponseDataInner]**](AppAnalyticsReportRequestsLinkagesResponseDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_analytics_report_requests_linkages_response import AppAnalyticsReportRequestsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppAnalyticsReportRequestsLinkagesResponse from a JSON string
app_analytics_report_requests_linkages_response_instance = AppAnalyticsReportRequestsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppAnalyticsReportRequestsLinkagesResponse.to_json())

# convert the object into a dict
app_analytics_report_requests_linkages_response_dict = app_analytics_report_requests_linkages_response_instance.to_dict()
# create an instance of AppAnalyticsReportRequestsLinkagesResponse from a dict
app_analytics_report_requests_linkages_response_from_dict = AppAnalyticsReportRequestsLinkagesResponse.from_dict(app_analytics_report_requests_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


