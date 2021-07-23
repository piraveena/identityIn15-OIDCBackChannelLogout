# OpenID Connect Back-channel logout samples

## Prerequisites
1. Install JDK8
2. Download apache tomcat 8
3. Add `localhost.com` in the `/etc/host` file.
3. Download and run WSO2 Identity Server 5.11.0
4. Download Pickup-dispatch and Pickup-manager samples ad deploy them in tomcat.
5. Register Pickup-dispatch and Pickup-manager in WSO2 Identity Server. Provides Callback URL for the application. Callback URLs of Pickup-dipatch and Pickup-Manager are given below.
```
Pickup-dispatch: http://localhost.com:8080/pickup-dispatch/oauth2client
Pickup-manager: http://localhost.com:8080/pickup-manager/oauth2client
```
6. Enable Back-channel logout for Pickup-dispatch and Pickup-manager. Provides back-channel logout URLs of Pickup-dipatch and Pickup-Manager  as shown below.
```
Pickup-dispatch: http://localhost.com:8080/pickup-dispatch/bclogout
Pickup-manager: http://localhost.com:8080/pickup-manager/bclogout
```

## Try out
1. Login to Pickup-dispatch.
2. WSO2 Identity Server will prompt with login page if you haven't logged in.
3. Enter the credentials and login to Pickup-dispatch.
4. Login to Pickup-manager.
5. You will be auto-logged into Pickup-manager.
6. Now tries to log out Pickup-dispatch.
7. Pickup Manager will be auto-logged out
