php-sms-rest
============

class for manage sms panel with php and rest
@ Kavenegar Api
@ Version: 2.0
@ Author: Javad Evazzadeh | Evazzadeh.com

Quick Start:
	copy this file in your project and edit KavenegarApi.php first line and insert your apikey and linenumber
	then copy and paste below line to quickly sent message!
		require("KavenegarApi.php");
		$api 	= new KavenegarApi();
		$result = $api->send('09120000000', 'Hi, This is for test!');


How to Use:
	for use this class you must require this file in your project with below line
		require("KavenegarApi.php");

	then you must create an instance from KavenegarApi with below line
		$api = new KavenegarApi();

	you can set the apikey and linenumber from declaration part of class in first lines
	but if you want you can set this parameter on create new instance with below code
		$api = new KavenegarApi('Your-apikey', 'Your-linenumber');

	for use the functions you can use below line sample, this line send message to 09120000000
		$result = $api->send('09120000000', 'Hi, This is for test!');
	
	if you want you can set the line number value after initializing class
		$api->linenumber = '100020003000';

	for access current status and server message you can read status value with below line
	var_dump($api->status);
	var_dump($api->msg);
