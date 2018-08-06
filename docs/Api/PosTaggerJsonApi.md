# Swagger\Client\PosTaggerJsonApi

All URIs are relative to *https://api.cloudmersive.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**posTaggerJsonPost**](PosTaggerJsonApi.md#posTaggerJsonPost) | **POST** /nlp/PosTaggerJson | Part-of-speech tag a string


# **posTaggerJsonPost**
> \Swagger\Client\Model\PosResponse posTaggerJsonPost($request)

Part-of-speech tag a string

Part-of-speech (POS) tag a string and return result as JSON

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\PosTaggerJsonApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$request = new \Swagger\Client\Model\PosRequest(); // \Swagger\Client\Model\PosRequest | Input string

try {
    $result = $apiInstance->posTaggerJsonPost($request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PosTaggerJsonApi->posTaggerJsonPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **request** | [**\Swagger\Client\Model\PosRequest**](../Model/PosRequest.md)| Input string |

### Return type

[**\Swagger\Client\Model\PosResponse**](../Model/PosResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json, text/json, application/xml, text/xml

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

