.. include:: ../links.rst

.. _Enable Social Sharing Icons:

############################
Enable Social Sharing Icons
############################

In the Open edX Cypress release, a new feature allows course staff to add
social sharing icons to their course listings in the LMS. Learners can select
these icons to create posts or tweets about their involvement in a course on
social sharing sites such as Facebook and Twitter without having to link their
accounts to these sites.

To use this feature on your instance of Open edX, you must configure dashboard
sharing settings. Optionally, you can configure custom course URLs and specify
a Social Sharing URL for your course page in Studio. If a custom course URL is
provided, the post or tweet by the social sharing site can provide a link back
to the URL location. If you do not configure custom course URLS, the URL to
the course About page in the LMS is used.

For information about social sharing icons, see the *Building and Running an
Open edX Course* guide.

.. note::  
   Before proceeding, review :ref:`Guidelines for Updating the edX Platform`.


.. _Configure Dashboard Sharing:

*******************************************************
Configure Dashboard Sharing
*******************************************************

To enable social sharing icons for a course, follow these steps to enable
dashboard share settings in both Studio and the LMS.


#. In the  ``/cms/envs/common.py`` and ``/lms/envs/common.py`` files, add the
   ``DASHBOARD_SHARE_SETTINGS`` and social sharing flags. 
   
   .. code-block:: bash

       # Dashboard share settings feature flag
        "DASHBOARD_SHARE_SETTINGS": {
            "FACEBOOK_SHARING": true,
            "TWITTER_SHARING": false,
            "TWITTER_SHARING_TEXT": 

2. For each social sharing icon that you want to enable, set the value of the
   setting to ``True``.

#. If you have set ``TWITTER_SHARING`` to ``True``, you can also specify
   default text that learners will see in the Twitter sharing dialog and that
   can be included in their tweet. Learners can edit this text before they
   select the **Share with Twitter** button in the LMS.

#. Save the ``/cms/envs/common.py`` and ``/lms/envs/common.py`` files.


*****************************************
Configure Custom Course URLs (Optional)
*****************************************

In addition to enabling the social sharing icons, if you want to provide a
custom URL for social sharing sites to link back to, follow these steps. You
must enable the setting in both Studio and the LMS, and specify the custom URL
in Studio **Advanced Settings**.

If you do not configure a custom course URL, the URL to the course About page
in the LMS is used.

	.. note:: If you add the ``CUSTOM_COURSE_URLS`` flag and set it to ``True``
	   but do not provide a value in the **Social Media Sharing URL** advanced
	   setting in Studio, social sharing icons are not visible in the LMS.


#. In the ``/cms/envs/common.py`` and ``/lms/envs/common.py`` files, add the
   ``CUSTOM_COURSE_URLS`` setting under ``DASHBOARD_SHARE_SETTINGS`` and set
   it to ``True``.
 
   .. code-block:: bash

       # Dashboard share settings feature flag
        "DASHBOARD_SHARE_SETTINGS": {
            "CUSTOM_COURSE_URLS": true,
            "FACEBOOK_SHARING": true,
            "TWITTER_SHARING": true,
            "TWITTER_SHARING_TEXT": Check out this fantastic course on edX!

#. Save the ``/cms/envs/common.py`` and ``/lms/envs/common.py`` files.

#. In Studio **Advanced Settings**, specify the custom course URL in the
   **Social Media Sharing URL** setting.

	This URL is provided to the social sharing site for linking back to a
	course location, such as the course About page. This URL is used only if
	you have :ref:`configured the dashboard share flags<Configure Dashboard
	Sharing>`.

	.. note:: If you add the ``CUSTOM_COURSE_URLS`` flag and set it to ``True``
	   but do not provide a value in the **Social Media Sharing URL** advanced
	   setting in Studio, social sharing icons are not visible in the LMS.

