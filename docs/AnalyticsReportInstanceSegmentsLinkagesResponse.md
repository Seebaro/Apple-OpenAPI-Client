# AnalyticsReportInstanceSegmentsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AnalyticsReportInstanceSegmentsLinkagesResponseDataInner]**](AnalyticsReportInstanceSegmentsLinkagesResponseDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.analytics_report_instance_segments_linkages_response import AnalyticsReportInstanceSegmentsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportInstanceSegmentsLinkagesResponse from a JSON string
analytics_report_instance_segments_linkages_response_instance = AnalyticsReportInstanceSegmentsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportInstanceSegmentsLinkagesResponse.to_json())

# convert the object into a dict
analytics_report_instance_segments_linkages_response_dict = analytics_report_instance_segments_linkages_response_instance.to_dict()
# create an instance of AnalyticsReportInstanceSegmentsLinkagesResponse from a dict
analytics_report_instance_segments_linkages_response_from_dict = AnalyticsReportInstanceSegmentsLinkagesResponse.from_dict(analytics_report_instance_segments_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


