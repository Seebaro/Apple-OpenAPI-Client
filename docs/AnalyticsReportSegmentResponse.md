# AnalyticsReportSegmentResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AnalyticsReportSegment**](AnalyticsReportSegment.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.analytics_report_segment_response import AnalyticsReportSegmentResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportSegmentResponse from a JSON string
analytics_report_segment_response_instance = AnalyticsReportSegmentResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportSegmentResponse.to_json())

# convert the object into a dict
analytics_report_segment_response_dict = analytics_report_segment_response_instance.to_dict()
# create an instance of AnalyticsReportSegmentResponse from a dict
analytics_report_segment_response_from_dict = AnalyticsReportSegmentResponse.from_dict(analytics_report_segment_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


