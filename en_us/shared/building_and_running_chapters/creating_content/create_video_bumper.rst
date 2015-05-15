.. _Adding a Bumper Video:

#####################################
Adding a Bumper Video to Your Course
#####################################

You can create a short video message and configure it to play before the other
videos in your course. For example, you can use the bumper video to provide
learners with information about your institution.

.. note:: Only courses that run on the edx.org website can include a bumper
 video. In addition, your institution must work with the edX media team to
 encode and host your video files. For more information, see `Processing Video
 Files`_.

.. contents:: Section Contents 
  :local:
  :depth: 1

**************************************
How Learners Experience a Bumper Video
**************************************

When a learner selects any video in the courseware, the defined course bumper
video might automatically begin to play before the selected video plays. The
bumper video does not play every time a learner plays any of the course
videos. Instead, it plays on an infrequent schedule. 

While the bumper video plays, the video player includes these additional
options for learners to select.

* **Skip**: The bumper video immediately stops playing and the selected video
  begins playing.
 
* **Do not show again**: The learner opts out of viewing this video, and it
  does not play for that learner again.

The following constraints control how the bumper video is delivered to
learners.

* For each enrolled learner, the bumper video plays a maximum of once every
  seven days.

* The bumper video plays only in web browsers. It does not play in the edX
  mobile app.

* The selected course video begins to play no more than 35 seconds after the
  learner selects it, even if the bumper video is longer than 35 seconds.

*****************************
Preparing the Bumper Video
*****************************

To include a bumper video in your course, you prepare the video file and its
transcript file or files and upload them to Studio. Because the bumper video
is not part of the courseware defined in the course outline, you do not use a
video component to add the bumper video to your course.

================================================
Create and Upload a Bumper Video File
================================================

Your bumper video can contain whatever content you want to include. The
following guidelines can help assure that the bumper video that you create
reaches as many learners as possible.

* The optimum length for a bumper video is 5 to 15 seconds. The video player
  stops playing longer files  after 35 seconds.

* Before you create a bumper video, be sure to review :ref:`Best Practices for
  Accessible Media`.

* The video must have at least one accompanying transcript. 

* The video must be in .mp4 or .mov format. For more information, see
  `Specifications for Successful Video Files`_ in the *Processing Video Files*
  guide.

After you create the file, you upload it on the Studio **Video Uploads** page.
The file goes through the automated encoding and hosting process, and is given
an identifying video ID. For more information, see `Upload Video Files`_ in
the *Processing Video Files* guide.

================================================
Prepare and Upload Bumper Video Transcript Files
================================================

To prepare the transcript files for a bumper video and upload them into
Studio, follow these steps.

#. On your local computer or network, locate the .srt transcript file or files
   for the bumper video.

   If your transcription service delivers your .srt files to YouTube, you must
   download the files from YouTube and save them locally.

#. Verify that each transcript file has a unique name. If you have transcript
   files in more than one language, be sure to include the ISO 639-1 language
   code as part of the file name. Example file names follow.

   ::
   
    edx_bumper_en.srt
    edx_bumper_es.srt
    edx_bumper_ru.srt

3. Open your course in Studio.

#. Select **Content**, and then **Files & Uploads**. 

#. Upload the files. For more information, see :ref:`Add Files to a Course`.

******************************************
Configuring a Bumper Video for Your Course
******************************************

To configure a video file and transcript files for your course bumper video,
you use an advanced setting in Studio. Because the bumper video is not part of
the courseware defined in the course outline, you do not use a video component
to add the bumper video to your course. You can identify only one file as the
video bumper at a time, but you can replace the file with a new one, or delete
the file, at any time.

.. contents:: Section Contents 
  :local:
  :depth: 1

======================================================
Identify the Bumper Video and Its Transcripts
======================================================

To identify the bumper video for your course, follow these steps.

#. Open three browser windows, and open your course in Studio in each one.

#. To obtain the video ID of the bumper video file, in one of the browser
   windows select **Content**, and then **Video Uploads**.

#. In another window you obtain the Studio URL of each transcript file. Select
   **Content**, and then **Files & Uploads** .

   .. note:: You identify the language of each transcript file with an 
    ISO 639-1 code. If your transcript file names do not already include 
    a language code, you will need a reference such as this 
    `list of ISO 639-1 codes`_.

#. In the last window, you define the course bumper video. Select **Settings**,
   and then **Advanced Settings**.

#. Scroll down to the **Video Bumper** policy key.

#. Between the braces in this field, enter ``"video_id":`` and then a space,
   followed by the ID value in quotation marks from the **Video Uploads**
   page.

   ::

     {"video_id": "83cef264-d6f5-4cf2-ad9d-0178ab8c92cd"}

7. After the closing quotation mark, add a comma and a space. 

   ::

     {"video_id": "83cef264-d6f5-4cf2-ad9d-0178ab8c92cd", }

8. After the comma and the space, enter ``"transcripts": {}``. 

#. Inside the pair of braces for the transcript, you enter a value pair to
   identify the language of the transcript file and then its Studio URL from
   the **Files & Uploads** page.

   ::

     {"video_id": "83cef264-d6f5-4cf2-ad9d-0178ab8c92cd", "transcripts": {"en": "/static/bumper_en.srt"}}
 
   You add the language code in quotation marks, followed by a colon and a
   space, and then add the URL in quotation marks.

10. If you have other transcript files, you add them in comma separated pairs
    after your first ``"language": "URL"`` pair.

    ::

      {"video_id": "83cef264-d6f5-4cf2-ad9d-0178ab8c92cd", "transcripts": {"en": "/static/bumper_en.srt", "zh": "/static/bumper_zh.srt"}}
 
11. Select **Save Changes**. Studio resequences and reformats your entry.
    Scroll back to **Video Bumper** to verify that your entry was saved as you
    expect. Entries that do not contain all of the required punctuation
    characters revert to the previous value when you save, and no warning is
    presented.

    ::

      {
          "transcripts": {
              "en": "/static/bumper_en.srt",
              "zh": "/static/bumper_zh.srt"
          },
          "video_id": "83cef264-d6f5-4cf2-ad9d-0178ab8c92cd"
      }

======================================================
Replace the Bumper Video and Its Transcripts
======================================================

You can change the bumper video for your course at any time. 

.. will students who opted not to watch a previous bumper see the new one?

To replace the bumper video for your course, follow these steps. 

#. Add the new bumper video file to your course on the **Video Uploads** page.

#. Add the transcript files for the bumper video on the **Files & Uploads**
   page.

#. On the **Advanced Settings** page, edit the **Video Bumper** policy key.

   #. Replace the previous video ID with the ID for the new bumper video file.

   #. Replace the previous transcript file URLs with the new Studio URLs. If
      needed, be sure to update the language codes for the transcripts.

4. Select **Save Changes**. 

===============================
Remove the Bumper Video
===============================

To remove the bumper file from your course, follow these steps. 

#. On the **Advanced Settings** page, delete the contents of the **Video
   Bumper** field.

#. Enter a pair of braces in the field. 
   
   ::

    {}

3. Select **Save Changes**. 


.. _Processing Video Files: http://processing-video-files.readthedocs.org/en/latest/
.. _Specifications for Successful Video Files: http://processing-video-files.readthedocs.org/en/latest/video_uploads.html#specifications-for-successful-video-files
.. _Upload Video Files: http://processing-video-files.readthedocs.org/en/latest/video_uploads.html#upload-video-files
.. _list of ISO 639-1 codes: http://en.wikipedia.org/wiki/List_of_ISO_639-1_codes