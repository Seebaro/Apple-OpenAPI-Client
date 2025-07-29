# AnalyticsReportInstancesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AnalyticsReportInstance]**](AnalyticsReportInstance.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.analytics_report_instances_response import AnalyticsReportInstancesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportInstancesResponse from a JSON string
analytics_report_instances_response_instance = AnalyticsReportInstancesResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportInstancesResponse.to_json())

# convert the object into a dict
analytics_report_instances_response_dict = analytics_report_instances_response_instance.to_dict()
# create an instance of AnalyticsReportInstancesResponse from a dict
analytics_report_instances_response_from_dict = AnalyticsReportInstancesResponse.from_dict(analytics_report_instances_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


