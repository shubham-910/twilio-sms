<h1 align="center">Magento_Twilio</h1> 

<div align="center">
  <p>Sends SMS messages in response to Magento events</p>
  <img src="https://img.shields.io/badge/magento-2.2%20|%202.3-brightgreen.svg?logo=magento&longCache=true&style=flat-square" alt="Supported Magento Versions" />
</div>

## Table of contents

- [Summary](#summary)

## Summary

There may be situations where you would like to be notified by SMS when a specific action happens within Magento. This module integrates with Twilio to provide that ability.

Currently implemented is a "pick & pack" SMS order notification which is sent in response to an order that has been placed.

## Installation

```
Download or clone this module in local machine
Then unzip or move it to the app/code.
php bin/magento module:enable Magento_Twilio
Above command is for enabling the module as we don't have any code to create any columns or table in the database.
php bin/magento setup:upgrade
And above command is to register and setup the module to use the functionality.
```

Retrieve your Account SID and Auth Token from the <a href="https://www.twilio.com/console" target="_blank">Twilio Console</a> Account Dashboard.

Enable the module and add Twilio credentials at Admin > Stores > Configuration > Twilio > General Configuration.

## Usage

Placing an order will result in an SMS message being sent.
