# BuildPerfPowerMetricsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppPerfPowerMetricsLinkagesResponseDataInner]**](AppPerfPowerMetricsLinkagesResponseDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.build_perf_power_metrics_linkages_response import BuildPerfPowerMetricsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BuildPerfPowerMetricsLinkagesResponse from a JSON string
build_perf_power_metrics_linkages_response_instance = BuildPerfPowerMetricsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(BuildPerfPowerMetricsLinkagesResponse.to_json())

# convert the object into a dict
build_perf_power_metrics_linkages_response_dict = build_perf_power_metrics_linkages_response_instance.to_dict()
# create an instance of BuildPerfPowerMetricsLinkagesResponse from a dict
build_perf_power_metrics_linkages_response_from_dict = BuildPerfPowerMetricsLinkagesResponse.from_dict(build_perf_power_metrics_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


