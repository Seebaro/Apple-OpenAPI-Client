# BuildBuildBetaDetailLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BuildRelationshipsBuildBetaDetailData**](BuildRelationshipsBuildBetaDetailData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.build_build_beta_detail_linkage_response import BuildBuildBetaDetailLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BuildBuildBetaDetailLinkageResponse from a JSON string
build_build_beta_detail_linkage_response_instance = BuildBuildBetaDetailLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(BuildBuildBetaDetailLinkageResponse.to_json())

# convert the object into a dict
build_build_beta_detail_linkage_response_dict = build_build_beta_detail_linkage_response_instance.to_dict()
# create an instance of BuildBuildBetaDetailLinkageResponse from a dict
build_build_beta_detail_linkage_response_from_dict = BuildBuildBetaDetailLinkageResponse.from_dict(build_build_beta_detail_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


