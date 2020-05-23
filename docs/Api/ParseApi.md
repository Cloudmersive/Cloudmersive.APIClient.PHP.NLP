# Swagger\Client\ParseApi

All URIs are relative to *https://api.cloudmersive.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**parseParseString**](ParseApi.md#parseParseString) | **POST** /nlp-v2/parse/tree | Parse string to syntax tree


# **parseParseString**
> \Swagger\Client\Model\ParseResponse parseParseString($input)

Parse string to syntax tree

Parses the input string into a Penn Treebank syntax tree

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\ParseApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$input = new \Swagger\Client\Model\ParseRequest(); // \Swagger\Client\Model\ParseRequest | Input string

try {
    $result = $apiInstance->parseParseString($input);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ParseApi->parseParseString: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **input** | [**\Swagger\Client\Model\ParseRequest**](../Model/ParseRequest.md)| Input string |

### Return type

[**\Swagger\Client\Model\ParseResponse**](../Model/ParseResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

