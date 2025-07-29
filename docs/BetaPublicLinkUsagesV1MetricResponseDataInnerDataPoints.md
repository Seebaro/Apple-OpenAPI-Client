# BetaPublicLinkUsagesV1MetricResponseDataInnerDataPoints


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**start** | **datetime** |  | [optional] 
**end** | **datetime** |  | [optional] 
**values** | [**BetaPublicLinkUsagesV1MetricResponseDataInnerDataPointsValues**](BetaPublicLinkUsagesV1MetricResponseDataInnerDataPointsValues.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_public_link_usages_v1_metric_response_data_inner_data_points import BetaPublicLinkUsagesV1MetricResponseDataInnerDataPoints

# TODO update the JSON string below
json = "{}"
# create an instance of BetaPublicLinkUsagesV1MetricResponseDataInnerDataPoints from a JSON string
beta_public_link_usages_v1_metric_response_data_inner_data_points_instance = BetaPublicLinkUsagesV1MetricResponseDataInnerDataPoints.from_json(json)
# print the JSON string representation of the object
print(BetaPublicLinkUsagesV1MetricResponseDataInnerDataPoints.to_json())

# convert the object into a dict
beta_public_link_usages_v1_metric_response_data_inner_data_points_dict = beta_public_link_usages_v1_metric_response_data_inner_data_points_instance.to_dict()
# create an instance of BetaPublicLinkUsagesV1MetricResponseDataInnerDataPoints from a dict
beta_public_link_usages_v1_metric_response_data_inner_data_points_from_dict = BetaPublicLinkUsagesV1MetricResponseDataInnerDataPoints.from_dict(beta_public_link_usages_v1_metric_response_data_inner_data_points_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


