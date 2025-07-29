# MetricsInsightPopulationsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**delta_percentage** | **float** |  | [optional] 
**percentile** | **str** |  | [optional] 
**summary_string** | **str** |  | [optional] 
**reference_average_value** | **float** |  | [optional] 
**latest_version_value** | **float** |  | [optional] 
**device** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.metrics_insight_populations_inner import MetricsInsightPopulationsInner

# TODO update the JSON string below
json = "{}"
# create an instance of MetricsInsightPopulationsInner from a JSON string
metrics_insight_populations_inner_instance = MetricsInsightPopulationsInner.from_json(json)
# print the JSON string representation of the object
print(MetricsInsightPopulationsInner.to_json())

# convert the object into a dict
metrics_insight_populations_inner_dict = metrics_insight_populations_inner_instance.to_dict()
# create an instance of MetricsInsightPopulationsInner from a dict
metrics_insight_populations_inner_from_dict = MetricsInsightPopulationsInner.from_dict(metrics_insight_populations_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


