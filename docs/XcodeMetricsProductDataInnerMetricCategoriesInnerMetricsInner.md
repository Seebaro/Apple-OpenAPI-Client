# XcodeMetricsProductDataInnerMetricCategoriesInnerMetricsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**identifier** | **str** |  | [optional] 
**goal_keys** | [**List[XcodeMetricsProductDataInnerMetricCategoriesInnerMetricsInnerGoalKeysInner]**](XcodeMetricsProductDataInnerMetricCategoriesInnerMetricsInnerGoalKeysInner.md) |  | [optional] 
**unit** | [**XcodeMetricsProductDataInnerMetricCategoriesInnerMetricsInnerUnit**](XcodeMetricsProductDataInnerMetricCategoriesInnerMetricsInnerUnit.md) |  | [optional] 
**datasets** | [**List[XcodeMetricsProductDataInnerMetricCategoriesInnerMetricsInnerDatasetsInner]**](XcodeMetricsProductDataInnerMetricCategoriesInnerMetricsInnerDatasetsInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.xcode_metrics_product_data_inner_metric_categories_inner_metrics_inner import XcodeMetricsProductDataInnerMetricCategoriesInnerMetricsInner

# TODO update the JSON string below
json = "{}"
# create an instance of XcodeMetricsProductDataInnerMetricCategoriesInnerMetricsInner from a JSON string
xcode_metrics_product_data_inner_metric_categories_inner_metrics_inner_instance = XcodeMetricsProductDataInnerMetricCategoriesInnerMetricsInner.from_json(json)
# print the JSON string representation of the object
print(XcodeMetricsProductDataInnerMetricCategoriesInnerMetricsInner.to_json())

# convert the object into a dict
xcode_metrics_product_data_inner_metric_categories_inner_metrics_inner_dict = xcode_metrics_product_data_inner_metric_categories_inner_metrics_inner_instance.to_dict()
# create an instance of XcodeMetricsProductDataInnerMetricCategoriesInnerMetricsInner from a dict
xcode_metrics_product_data_inner_metric_categories_inner_metrics_inner_from_dict = XcodeMetricsProductDataInnerMetricCategoriesInnerMetricsInner.from_dict(xcode_metrics_product_data_inner_metric_categories_inner_metrics_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


