# CiProductBuildRunsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiBuildActionRelationshipsBuildRunData]**](CiBuildActionRelationshipsBuildRunData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_product_build_runs_linkages_response import CiProductBuildRunsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiProductBuildRunsLinkagesResponse from a JSON string
ci_product_build_runs_linkages_response_instance = CiProductBuildRunsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(CiProductBuildRunsLinkagesResponse.to_json())

# convert the object into a dict
ci_product_build_runs_linkages_response_dict = ci_product_build_runs_linkages_response_instance.to_dict()
# create an instance of CiProductBuildRunsLinkagesResponse from a dict
ci_product_build_runs_linkages_response_from_dict = CiProductBuildRunsLinkagesResponse.from_dict(ci_product_build_runs_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


