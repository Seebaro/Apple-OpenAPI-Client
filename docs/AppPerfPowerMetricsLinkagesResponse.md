# AppPerfPowerMetricsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppPerfPowerMetricsLinkagesResponseDataInner]**](AppPerfPowerMetricsLinkagesResponseDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_perf_power_metrics_linkages_response import AppPerfPowerMetricsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppPerfPowerMetricsLinkagesResponse from a JSON string
app_perf_power_metrics_linkages_response_instance = AppPerfPowerMetricsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppPerfPowerMetricsLinkagesResponse.to_json())

# convert the object into a dict
app_perf_power_metrics_linkages_response_dict = app_perf_power_metrics_linkages_response_instance.to_dict()
# create an instance of AppPerfPowerMetricsLinkagesResponse from a dict
app_perf_power_metrics_linkages_response_from_dict = AppPerfPowerMetricsLinkagesResponse.from_dict(app_perf_power_metrics_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


