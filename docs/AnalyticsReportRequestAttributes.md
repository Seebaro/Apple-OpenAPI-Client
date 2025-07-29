# AnalyticsReportRequestAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**access_type** | **str** |  | [optional] 
**stopped_due_to_inactivity** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.analytics_report_request_attributes import AnalyticsReportRequestAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportRequestAttributes from a JSON string
analytics_report_request_attributes_instance = AnalyticsReportRequestAttributes.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportRequestAttributes.to_json())

# convert the object into a dict
analytics_report_request_attributes_dict = analytics_report_request_attributes_instance.to_dict()
# create an instance of AnalyticsReportRequestAttributes from a dict
analytics_report_request_attributes_from_dict = AnalyticsReportRequestAttributes.from_dict(analytics_report_request_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


