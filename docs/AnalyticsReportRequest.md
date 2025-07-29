# AnalyticsReportRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AnalyticsReportRequestAttributes**](AnalyticsReportRequestAttributes.md) |  | [optional] 
**relationships** | [**AnalyticsReportRequestRelationships**](AnalyticsReportRequestRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.analytics_report_request import AnalyticsReportRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportRequest from a JSON string
analytics_report_request_instance = AnalyticsReportRequest.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportRequest.to_json())

# convert the object into a dict
analytics_report_request_dict = analytics_report_request_instance.to_dict()
# create an instance of AnalyticsReportRequest from a dict
analytics_report_request_from_dict = AnalyticsReportRequest.from_dict(analytics_report_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


