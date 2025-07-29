# AnalyticsReport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AnalyticsReportAttributes**](AnalyticsReportAttributes.md) |  | [optional] 
**relationships** | [**AnalyticsReportRelationships**](AnalyticsReportRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.analytics_report import AnalyticsReport

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReport from a JSON string
analytics_report_instance = AnalyticsReport.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReport.to_json())

# convert the object into a dict
analytics_report_dict = analytics_report_instance.to_dict()
# create an instance of AnalyticsReport from a dict
analytics_report_from_dict = AnalyticsReport.from_dict(analytics_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


