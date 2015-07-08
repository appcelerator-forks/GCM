# CaffeinaGCM

### Google Cloud Messaging support

#### Register for Push notifications

```js
require('it.caffeina.gcm').registerForPushNotifications({
	senderId: 'XXXXXXXXXXXX',
	callback: function(e) {

		// Here you have the payload

	},
	success: function(e) {
		console.log(e);
	},
	error: function(err) {
		Ti.API.error('Notifications: Retrieve device token failed', err);
	}
});
```


#### Unregister

```js
require('it.caffeina.gcm').unregisterForPushNotifications();
```