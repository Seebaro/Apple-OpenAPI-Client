# AnalyticsReportInstance


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AnalyticsReportInstanceAttributes**](AnalyticsReportInstanceAttributes.md) |  | [optional] 
**relationships** | [**AnalyticsReportInstanceRelationships**](AnalyticsReportInstanceRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.analytics_report_instance import AnalyticsReportInstance

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportInstance from a JSON string
analytics_report_instance_instance = AnalyticsReportInstance.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportInstance.to_json())

# convert the object into a dict
analytics_report_instance_dict = analytics_report_instance_instance.to_dict()
# create an instance of AnalyticsReportInstance from a dict
analytics_report_instance_from_dict = AnalyticsReportInstance.from_dict(analytics_report_instance_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


