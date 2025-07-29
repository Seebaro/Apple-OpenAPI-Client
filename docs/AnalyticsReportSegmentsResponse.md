# AnalyticsReportSegmentsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AnalyticsReportSegment]**](AnalyticsReportSegment.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.analytics_report_segments_response import AnalyticsReportSegmentsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportSegmentsResponse from a JSON string
analytics_report_segments_response_instance = AnalyticsReportSegmentsResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportSegmentsResponse.to_json())

# convert the object into a dict
analytics_report_segments_response_dict = analytics_report_segments_response_instance.to_dict()
# create an instance of AnalyticsReportSegmentsResponse from a dict
analytics_report_segments_response_from_dict = AnalyticsReportSegmentsResponse.from_dict(analytics_report_segments_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


