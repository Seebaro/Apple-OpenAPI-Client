# AnalyticsReportInstancesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AnalyticsReportInstancesLinkagesResponseDataInner]**](AnalyticsReportInstancesLinkagesResponseDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.analytics_report_instances_linkages_response import AnalyticsReportInstancesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportInstancesLinkagesResponse from a JSON string
analytics_report_instances_linkages_response_instance = AnalyticsReportInstancesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportInstancesLinkagesResponse.to_json())

# convert the object into a dict
analytics_report_instances_linkages_response_dict = analytics_report_instances_linkages_response_instance.to_dict()
# create an instance of AnalyticsReportInstancesLinkagesResponse from a dict
analytics_report_instances_linkages_response_from_dict = AnalyticsReportInstancesLinkagesResponse.from_dict(analytics_report_instances_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


