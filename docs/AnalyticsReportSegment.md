# AnalyticsReportSegment


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AnalyticsReportSegmentAttributes**](AnalyticsReportSegmentAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.analytics_report_segment import AnalyticsReportSegment

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportSegment from a JSON string
analytics_report_segment_instance = AnalyticsReportSegment.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportSegment.to_json())

# convert the object into a dict
analytics_report_segment_dict = analytics_report_segment_instance.to_dict()
# create an instance of AnalyticsReportSegment from a dict
analytics_report_segment_from_dict = AnalyticsReportSegment.from_dict(analytics_report_segment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


