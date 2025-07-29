# XcodeMetricsProductDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**platform** | **str** |  | [optional] 
**metric_categories** | [**List[XcodeMetricsProductDataInnerMetricCategoriesInner]**](XcodeMetricsProductDataInnerMetricCategoriesInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.xcode_metrics_product_data_inner import XcodeMetricsProductDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of XcodeMetricsProductDataInner from a JSON string
xcode_metrics_product_data_inner_instance = XcodeMetricsProductDataInner.from_json(json)
# print the JSON string representation of the object
print(XcodeMetricsProductDataInner.to_json())

# convert the object into a dict
xcode_metrics_product_data_inner_dict = xcode_metrics_product_data_inner_instance.to_dict()
# create an instance of XcodeMetricsProductDataInner from a dict
xcode_metrics_product_data_inner_from_dict = XcodeMetricsProductDataInner.from_dict(xcode_metrics_product_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


