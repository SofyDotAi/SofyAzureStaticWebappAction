# Sofy Azure Webapp Integration

Sofy for Web integrates into your Azure Static Webapp CI/CD pipeline through Github actions. Sofy will monitor your website and send you exploratory testing results after every push with no input required.

To learn more about Sofy For Web click [here](https://sofy.ai/azure-static-webapp-integration/) 

## Prerequisites

In order to integrate your Azure Static Webapp with Sofy for Web, you need to first create an account with Sofy. 

1. [Create an Account with Sofy Here](https://sofy.ai/register/)
2. Once your account is created, click on the tab *I want to test a Website*
	![Test a Website](newaccount.png)


## Inputs

### `website_url`

**Required** The url endpoint of your website. Default `""`.

### `application_guid`

**Required** ApplicationGUID retrieved from SOFY for Web `""`.

### `application_id`

**Required** ApplicationID retrieved from SOFY for Web `""`.

## Outputs

### `time`

The time we created the run you.

## Example usage

uses: actions/#Sofy_ASW_Action@v1.1
with:
  website_url: 'https://www.ebay.com'
  application_guid: <GUID Obtained from Sofy>
  application_id: '<APPID Obtained from Sofy>
