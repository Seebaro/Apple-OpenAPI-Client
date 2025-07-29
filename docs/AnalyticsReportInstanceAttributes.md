# AnalyticsReportInstanceAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**granularity** | **str** |  | [optional] 
**processing_date** | **date** |  | [optional] 

## Example

```python
from openapi_client.models.analytics_report_instance_attributes import AnalyticsReportInstanceAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportInstanceAttributes from a JSON string
analytics_report_instance_attributes_instance = AnalyticsReportInstanceAttributes.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportInstanceAttributes.to_json())

# convert the object into a dict
analytics_report_instance_attributes_dict = analytics_report_instance_attributes_instance.to_dict()
# create an instance of AnalyticsReportInstanceAttributes from a dict
analytics_report_instance_attributes_from_dict = AnalyticsReportInstanceAttributes.from_dict(analytics_report_instance_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


