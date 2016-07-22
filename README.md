# google-firebase-login

This component will log you in  Google and will reuse the oauth token to log you in your firebae app. 

You need a firebase-app component somewhere in your app

As described in https://developers.google.com/identity/protocols/OAuth2InstalledApp your secret key is not supposed to be secret for installed apps.

You will need InAppBrowser plugin when packing your app.


```html

  <firebase-app auth-domain="your-firebase-app" database-url="your-firebase-db" api-key="your-firebase-key">

  <google-firebase-login clientIdWeb="your-client-id-web" clientId="your-client-id-native" clientSecret="your-secret-key-native">
  </google-firebase-login>

```