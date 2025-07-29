# AnalyticsReportAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**category** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.analytics_report_attributes import AnalyticsReportAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportAttributes from a JSON string
analytics_report_attributes_instance = AnalyticsReportAttributes.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportAttributes.to_json())

# convert the object into a dict
analytics_report_attributes_dict = analytics_report_attributes_instance.to_dict()
# create an instance of AnalyticsReportAttributes from a dict
analytics_report_attributes_from_dict = AnalyticsReportAttributes.from_dict(analytics_report_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


