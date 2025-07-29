# XcodeMetricsInsights


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**trending_up** | [**List[MetricsInsight]**](MetricsInsight.md) |  | [optional] 
**regressions** | [**List[MetricsInsight]**](MetricsInsight.md) |  | [optional] 

## Example

```python
from openapi_client.models.xcode_metrics_insights import XcodeMetricsInsights

# TODO update the JSON string below
json = "{}"
# create an instance of XcodeMetricsInsights from a JSON string
xcode_metrics_insights_instance = XcodeMetricsInsights.from_json(json)
# print the JSON string representation of the object
print(XcodeMetricsInsights.to_json())

# convert the object into a dict
xcode_metrics_insights_dict = xcode_metrics_insights_instance.to_dict()
# create an instance of XcodeMetricsInsights from a dict
xcode_metrics_insights_from_dict = XcodeMetricsInsights.from_dict(xcode_metrics_insights_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


