# openapi_client.BetaRecruitmentCriterionOptionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**beta_recruitment_criterion_options_get_collection**](BetaRecruitmentCriterionOptionsApi.md#beta_recruitment_criterion_options_get_collection) | **GET** /v1/betaRecruitmentCriterionOptions | 


# **beta_recruitment_criterion_options_get_collection**
> BetaRecruitmentCriterionOptionsResponse beta_recruitment_criterion_options_get_collection(fields_beta_recruitment_criterion_options=fields_beta_recruitment_criterion_options, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_recruitment_criterion_options_response import BetaRecruitmentCriterionOptionsResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.BetaRecruitmentCriterionOptionsApi(api_client)
    fields_beta_recruitment_criterion_options = ['fields_beta_recruitment_criterion_options_example'] # List[str] | the fields to include for returned resources of type betaRecruitmentCriterionOptions (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.beta_recruitment_criterion_options_get_collection(fields_beta_recruitment_criterion_options=fields_beta_recruitment_criterion_options, limit=limit)
        print("The response of BetaRecruitmentCriterionOptionsApi->beta_recruitment_criterion_options_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BetaRecruitmentCriterionOptionsApi->beta_recruitment_criterion_options_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields_beta_recruitment_criterion_options** | [**List[str]**](str.md)| the fields to include for returned resources of type betaRecruitmentCriterionOptions | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**BetaRecruitmentCriterionOptionsResponse**](BetaRecruitmentCriterionOptionsResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**200** | List of BetaRecruitmentCriterionOptions |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

