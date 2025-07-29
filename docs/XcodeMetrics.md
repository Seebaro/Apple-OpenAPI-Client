# XcodeMetrics


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**version** | **str** |  | [optional] 
**insights** | [**XcodeMetricsInsights**](XcodeMetricsInsights.md) |  | [optional] 
**product_data** | [**List[XcodeMetricsProductDataInner]**](XcodeMetricsProductDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.xcode_metrics import XcodeMetrics

# TODO update the JSON string below
json = "{}"
# create an instance of XcodeMetrics from a JSON string
xcode_metrics_instance = XcodeMetrics.from_json(json)
# print the JSON string representation of the object
print(XcodeMetrics.to_json())

# convert the object into a dict
xcode_metrics_dict = xcode_metrics_instance.to_dict()
# create an instance of XcodeMetrics from a dict
xcode_metrics_from_dict = XcodeMetrics.from_dict(xcode_metrics_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


