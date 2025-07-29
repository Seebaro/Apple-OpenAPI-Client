# XcodeMetricsProductDataInnerMetricCategoriesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**identifier** | [**MetricCategory**](MetricCategory.md) |  | [optional] 
**metrics** | [**List[XcodeMetricsProductDataInnerMetricCategoriesInnerMetricsInner]**](XcodeMetricsProductDataInnerMetricCategoriesInnerMetricsInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.xcode_metrics_product_data_inner_metric_categories_inner import XcodeMetricsProductDataInnerMetricCategoriesInner

# TODO update the JSON string below
json = "{}"
# create an instance of XcodeMetricsProductDataInnerMetricCategoriesInner from a JSON string
xcode_metrics_product_data_inner_metric_categories_inner_instance = XcodeMetricsProductDataInnerMetricCategoriesInner.from_json(json)
# print the JSON string representation of the object
print(XcodeMetricsProductDataInnerMetricCategoriesInner.to_json())

# convert the object into a dict
xcode_metrics_product_data_inner_metric_categories_inner_dict = xcode_metrics_product_data_inner_metric_categories_inner_instance.to_dict()
# create an instance of XcodeMetricsProductDataInnerMetricCategoriesInner from a dict
xcode_metrics_product_data_inner_metric_categories_inner_from_dict = XcodeMetricsProductDataInnerMetricCategoriesInner.from_dict(xcode_metrics_product_data_inner_metric_categories_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


