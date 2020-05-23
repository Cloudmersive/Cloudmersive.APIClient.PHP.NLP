# Swagger\Client\SpellcheckApi

All URIs are relative to *https://api.cloudmersive.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**spellcheckCheckSentence**](SpellcheckApi.md#spellcheckCheckSentence) | **POST** /nlp-v2/spellcheck/check/sentence | Check if sentence is spelled correctly
[**spellcheckCorrectJson**](SpellcheckApi.md#spellcheckCorrectJson) | **POST** /nlp-v2/spellcheck/check/word | Find spelling corrections


# **spellcheckCheckSentence**
> \Swagger\Client\Model\CheckSentenceResponse spellcheckCheckSentence($value)

Check if sentence is spelled correctly

Checks whether the sentence is spelled correctly and returns the result as JSON

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\SpellcheckApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = new \Swagger\Client\Model\CheckSentenceRequest(); // \Swagger\Client\Model\CheckSentenceRequest | Input sentence

try {
    $result = $apiInstance->spellcheckCheckSentence($value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SpellcheckApi->spellcheckCheckSentence: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | [**\Swagger\Client\Model\CheckSentenceRequest**](../Model/CheckSentenceRequest.md)| Input sentence |

### Return type

[**\Swagger\Client\Model\CheckSentenceResponse**](../Model/CheckSentenceResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **spellcheckCorrectJson**
> \Swagger\Client\Model\CheckWordResponse spellcheckCorrectJson($value)

Find spelling corrections

Find spelling correction suggestions and return result as JSON

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\SpellcheckApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = new \Swagger\Client\Model\CheckWordRequest(); // \Swagger\Client\Model\CheckWordRequest | Input string

try {
    $result = $apiInstance->spellcheckCorrectJson($value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SpellcheckApi->spellcheckCorrectJson: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | [**\Swagger\Client\Model\CheckWordRequest**](../Model/CheckWordRequest.md)| Input string |

### Return type

[**\Swagger\Client\Model\CheckWordResponse**](../Model/CheckWordResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

