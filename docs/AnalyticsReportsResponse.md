# AnalyticsReportsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AnalyticsReport]**](AnalyticsReport.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.analytics_reports_response import AnalyticsReportsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsReportsResponse from a JSON string
analytics_reports_response_instance = AnalyticsReportsResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsReportsResponse.to_json())

# convert the object into a dict
analytics_reports_response_dict = analytics_reports_response_instance.to_dict()
# create an instance of AnalyticsReportsResponse from a dict
analytics_reports_response_from_dict = AnalyticsReportsResponse.from_dict(analytics_reports_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


