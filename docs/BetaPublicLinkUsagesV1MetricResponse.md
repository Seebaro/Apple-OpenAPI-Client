# BetaPublicLinkUsagesV1MetricResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BetaPublicLinkUsagesV1MetricResponseDataInner]**](BetaPublicLinkUsagesV1MetricResponseDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_public_link_usages_v1_metric_response import BetaPublicLinkUsagesV1MetricResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaPublicLinkUsagesV1MetricResponse from a JSON string
beta_public_link_usages_v1_metric_response_instance = BetaPublicLinkUsagesV1MetricResponse.from_json(json)
# print the JSON string representation of the object
print(BetaPublicLinkUsagesV1MetricResponse.to_json())

# convert the object into a dict
beta_public_link_usages_v1_metric_response_dict = beta_public_link_usages_v1_metric_response_instance.to_dict()
# create an instance of BetaPublicLinkUsagesV1MetricResponse from a dict
beta_public_link_usages_v1_metric_response_from_dict = BetaPublicLinkUsagesV1MetricResponse.from_dict(beta_public_link_usages_v1_metric_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


