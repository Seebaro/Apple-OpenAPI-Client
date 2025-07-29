# AppsBetaTesterUsagesV1MetricResponseDataInnerDataPoints


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**start** | **datetime** |  | [optional] 
**end** | **datetime** |  | [optional] 
**values** | [**AppsBetaTesterUsagesV1MetricResponseDataInnerDataPointsValues**](AppsBetaTesterUsagesV1MetricResponseDataInnerDataPointsValues.md) |  | [optional] 

## Example

```python
from openapi_client.models.apps_beta_tester_usages_v1_metric_response_data_inner_data_points import AppsBetaTesterUsagesV1MetricResponseDataInnerDataPoints

# TODO update the JSON string below
json = "{}"
# create an instance of AppsBetaTesterUsagesV1MetricResponseDataInnerDataPoints from a JSON string
apps_beta_tester_usages_v1_metric_response_data_inner_data_points_instance = AppsBetaTesterUsagesV1MetricResponseDataInnerDataPoints.from_json(json)
# print the JSON string representation of the object
print(AppsBetaTesterUsagesV1MetricResponseDataInnerDataPoints.to_json())

# convert the object into a dict
apps_beta_tester_usages_v1_metric_response_data_inner_data_points_dict = apps_beta_tester_usages_v1_metric_response_data_inner_data_points_instance.to_dict()
# create an instance of AppsBetaTesterUsagesV1MetricResponseDataInnerDataPoints from a dict
apps_beta_tester_usages_v1_metric_response_data_inner_data_points_from_dict = AppsBetaTesterUsagesV1MetricResponseDataInnerDataPoints.from_dict(apps_beta_tester_usages_v1_metric_response_data_inner_data_points_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


