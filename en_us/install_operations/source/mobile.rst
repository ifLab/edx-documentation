.. include:: links.rst

.. _Setting up the Mobile Applications:

######################################
Setting up the edX Mobile Applications
######################################

This section is intended for those are who are building the edX mobile
applications and customizing their Open edX installation to support their use.

.. contents:: Section Contents 
   :local:

.. Mark, this option ^ prevents the section name from appearing as a link. What do you think about standardizing on this format at the beginning of each rst? 

******************************
Accessing the Source Code
******************************

There are currently two edX mobile applications, one for iOS and one for
Android. You can find the source code and additional documentation for each
application here.

* iOS: http://github.com/edx/edx-app-ios

* Android: http://github.com/edx/edx-app-android

*****************************************
Configuring Mobile Application Features
*****************************************

For the mobile API, authentication, and other features to work correctly with
the edX mobile applications, you enable them.

* You can enable the features temporarily in the ``lms.env.json`` file.
  Configuration settings added to this file are reset to their default values
  each time you update ``edx-platform``.

* You can also define the configuration that you want in the 
  ``server-vars.yml`` file. Configuration settings made in this file are 
  reapplied automatically when you update ``edx-platform``.

After you enable the features, you add an OAuth client.

====================================
Enable Features in ``lms.env.json``
====================================

You can enable the mobile application features in the ``lms.env.json`` file.
Configuration settings added to this file are reset to their default values
each time you update edx-platform.

#. In the ``edx/app/edxapp/lms.env.json`` file, add the following lines to the
   features section.

   .. code-block:: json

       "FEATURES" : {
           ...
           "ENABLE_MOBILE_REST_API": true,
           "ENABLE_OAUTH2_PROVIDER": true,
           "ENABLE_THIRD_PARTY_AUTH": true,
           "ENABLE_COMBINED_LOGIN_REGISTRATION": true
       }

#. To complete configuration of OAuth2 authentication, add the following line
   at the top level of the configuration dictionary. 

   .. code-block:: json

       "OAUTH_ENFORCE_SECURE": " ",

   For example, you can add this line immediately after the closing
   parenthesis for the Features section.

#. Save the ``edx/app/edxapp/lms.env.json`` file.

#. Restart the server.

=======================================
Enable Features in ``server-vars.yml``
=======================================

You can enable many of the mobile application features in the 
``server-vars.yml`` file. Configuration settings added to this file 
are reapplied automatically when you update ``edx-platform``.
   
.. note:: Currently, you must manually add 
          ``"OAUTH_ENFORCE_SECURE": " ",`` to the
          ``edx/app/edxapp/lms.env.json`` file.

#. In the ``/edx/app/edx_ansible/server-vars.yml`` file, add the following
   lines to the edX app features section.

   .. code-block:: json

       EDXAPP_FEATURES:
         ENABLE_MOBILE_REST_API: true
         ENABLE_OAUTH2_PROVIDER: true
         ENABLE_VIDEO_UPLOAD_PIPELINE: true
         ENABLE_THIRD_PARTY_AUTH: true
         ENABLE_COMBINED_LOGIN_REGISTRATION: true

#. Save the ``/edx/app/edx_ansible/server-vars.yml`` file.

=======================================
Create a Client for Authentication 
=======================================

You create an OAuth key and secret that is specific to 
your installation for use by the mobile applications. 

#. Log in to the Django administration console at ``<YOUR_EDX_INSTALLATION>/admin``. 

#. In the **Oauth2** section, select **Clients**. 

#. Select **Add client** and create a client.

#. Add the ID and the secret for the client to your custom configuration. For
   information about how to set up your custom configuration, see the GitHub
   repository for `iOS`_ or `Android`_.

************************************
Configuring Video Modules for Mobile
************************************

Courseware videos must be specifically prepared to ensure that they are in
mobile accessible formats. Video modules in mobile-available courses should
have low resolution encodings that are readily accessible by mobile
devices.

To configure a video module with a low resolution encoding for mobile in edX
Studio, you edit the video component. On the **Advanced** tab, in the **Video
File URLs** field, enter the URL to the mobile-targeted video as the first URL
in the list. For more information, see `Working with Video Components`_ in
*Building and Running an Open edX Course*.

Alternatively, if you edit the course directly in XML, enter the URL to the
mobile-targeted video as the first URL in the list of ``html5_sources``. For
more information, see `Video Components`_ in the *edX Open Learning XML
Guide*.

****************************************
Enable Push Notification 
****************************************

You enable push notification by configuring both the ``edx-platform``
repository and the edX mobile applications.

============================================
Set Up Your Open edX Platform Repository  
============================================

To send push notifications from edX Studio to the edX mobile applications, you
install the ``edx_notifications`` application and customize its configuration
to identify your push messaging service or push notification server.

For more information, see https://github.com/edx/edx-notifications.

================================================================
Configure Push Notification in Your Open edX Mobile Applications
================================================================

For the edX mobile applications, the ``PUSH_NOTIFICATIONS`` key enables push
notification support.

If you are using Parse to provide notification delivery, you also add the
following keys.

::

    PARSE:
      NOTIFICATIONS_ENABLED: true
      APPLICATION_ID: {your application id}
      CLIENT_KEY: {your client key}


Configure the edX Mobile Application for iOS
************************************************

To use a push notification service other than Parse with with your edX Mobile
Application for iOS, you implement the `OEXPushProvider.h`_ protocol.

The following classes are used for push notifications.

* The `OEXParsePushProvider.m`_ class handles Parse setup.

* The `OEXPushNotificationManager.m`_ class handles push registration and
  dispatch.

Configure the edX Mobile Application for Android
************************************************

To use Parse for push notification services with your edX Mobile Application
for Android, you update the `AndroidManifest.xml`_ manifest file.

The following classes are used for push notifications.

* The `EdxParsePushBroadcastReceiver.java`_ class intercepts Parse
  notification events and adds custom behaviors.

* The `UserNotificationManager.java`_ class handles push registration and
  dispatch.

* The `ParseNotificationDelegate.java`_ class handles Parse registration.
