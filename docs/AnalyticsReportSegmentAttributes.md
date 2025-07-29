# AnalyticsReportSegmentAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**checksum** | **str** |  | [optional] 
**size_in_bytes** | **int** |  | [optional] 
**url** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.analytics_report_segment_attributes import AnalyticsReportSegmentAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportSegmentAttributes from a JSON string
analytics_report_segment_attributes_instance = AnalyticsReportSegmentAttributes.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportSegmentAttributes.to_json())

# convert the object into a dict
analytics_report_segment_attributes_dict = analytics_report_segment_attributes_instance.to_dict()
# create an instance of AnalyticsReportSegmentAttributes from a dict
analytics_report_segment_attributes_from_dict = AnalyticsReportSegmentAttributes.from_dict(analytics_report_segment_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


