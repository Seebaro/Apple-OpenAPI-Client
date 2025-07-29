# MetricsInsight


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metric_category** | [**MetricCategory**](MetricCategory.md) |  | [optional] 
**latest_version** | **str** |  | [optional] 
**metric** | **str** |  | [optional] 
**summary_string** | **str** |  | [optional] 
**reference_versions** | **str** |  | [optional] 
**max_latest_version_value** | **float** |  | [optional] 
**sub_system_label** | **str** |  | [optional] 
**high_impact** | **bool** |  | [optional] 
**populations** | [**List[MetricsInsightPopulationsInner]**](MetricsInsightPopulationsInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.metrics_insight import MetricsInsight

# TODO update the JSON string below
json = "{}"
# create an instance of MetricsInsight from a JSON string
metrics_insight_instance = MetricsInsight.from_json(json)
# print the JSON string representation of the object
print(MetricsInsight.to_json())

# convert the object into a dict
metrics_insight_dict = metrics_insight_instance.to_dict()
# create an instance of MetricsInsight from a dict
metrics_insight_from_dict = MetricsInsight.from_dict(metrics_insight_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


