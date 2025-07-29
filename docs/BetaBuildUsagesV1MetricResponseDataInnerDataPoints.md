# BetaBuildUsagesV1MetricResponseDataInnerDataPoints


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**start** | **datetime** |  | [optional] 
**end** | **datetime** |  | [optional] 
**values** | [**BetaBuildUsagesV1MetricResponseDataInnerDataPointsValues**](BetaBuildUsagesV1MetricResponseDataInnerDataPointsValues.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_build_usages_v1_metric_response_data_inner_data_points import BetaBuildUsagesV1MetricResponseDataInnerDataPoints

# TODO update the JSON string below
json = "{}"
# create an instance of BetaBuildUsagesV1MetricResponseDataInnerDataPoints from a JSON string
beta_build_usages_v1_metric_response_data_inner_data_points_instance = BetaBuildUsagesV1MetricResponseDataInnerDataPoints.from_json(json)
# print the JSON string representation of the object
print(BetaBuildUsagesV1MetricResponseDataInnerDataPoints.to_json())

# convert the object into a dict
beta_build_usages_v1_metric_response_data_inner_data_points_dict = beta_build_usages_v1_metric_response_data_inner_data_points_instance.to_dict()
# create an instance of BetaBuildUsagesV1MetricResponseDataInnerDataPoints from a dict
beta_build_usages_v1_metric_response_data_inner_data_points_from_dict = BetaBuildUsagesV1MetricResponseDataInnerDataPoints.from_dict(beta_build_usages_v1_metric_response_data_inner_data_points_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


