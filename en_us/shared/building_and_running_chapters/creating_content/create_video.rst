.. _Working with Video Components:

#############################
创建影片组件
#############################

您能创建一个您的演讲影片，并且可以将其他组成部分，例如，讨论和遇到的问题，添加到课程中是学生积极学习。
将视频添加到您的课程中有以下几个步骤。

.. contents:: Section Contents
  :local:
  :depth: 1

.. note:: 在将影片添加到您的课程之前，回顾 :ref:`Best Practices for Accessible Media` 。

.. _Protecting Videos:

************************
Protecting Videos
************************ 

To help course teams protect video assets, the edX video player hides video
URLs from learners by default. This functionality is in effect for all video
files, including YouTube videos and videos that you have posted in other
locations. Learners can still download videos if you select the **Video
Download Allowed** option for your video components. For more information about
posting videos not hosted on YouTube, see :ref:`Post the Video Online`. For
more information about options that you can set when you create a video
component, see :ref:`Video Advanced Options`.

.. _Create the Video:

************************
步骤1. 创建影片
************************

您的影片能保存任何您想要保存的内容。`edX101 Overview of Creating an edX Course`_ 中的
`Creating Videos`_ 部分能够帮助您如何创建影片内容。

.. _Compression Specifications:

====================================
压缩详述
====================================

创建影片时，edX建议参照以下压缩详述。

.. list-table::
   :widths: 10 20 20
   :stub-columns: 1

   * - Output
     - **Publish to YouTube**
     - **Publish downloadable file to AWS S3**
   * - Codec
     - H.264 .mp4
     - H.264 .mp4
   * - Resolution & Frame Rate (see note)
     - 1920x1080, progressive, 29.97 fps
     - 1280x720, progressive, 29.97 fps
   * - Aspect
     - 1.0
     - 1.0
   * - Bit Rate
     - VBR, 2 pass
     - VBR, 2 pass
   * - Target VBR
     - 5 mbps
     - 1 mbps
   * - Max VBR
     - 7.5 mbps
     - 1.5 mbps
   * - Audio
     - AAC 44.1 / 192 kbps
     - AAC 44.1 / 192 kbps

.. note:: Typically you export at the same frame rate that was used when you
 created the media file. For example, if you create the file in a country that
 uses the PAL system, you export at 25 fps instead of the NTSC standard of
 29.97 fps.

.. _Video Formats:

==================
影片格式
==================

edX视频播放器支持mp4, .webm, .mpeg, and .ogg格式。
然而，为了确保所有标准浏览器均能播放您的影片， 我们强烈建议您使用 **.mp4 format** 格式。

.. _Create Transcript:

*********************************************
步骤2. 创建或保存影片字幕
*********************************************

我们强烈建议您将影片与有限的字幕相结合。
对于那些母语是非英语、不能看见影片或这想要回顾影片内容的学生来说，字幕对他们是十分有用的。
您的影片播放的同时字幕也会自动滚动播放。要是学生点击字幕中的单词，影片会显示该词。
您能让学生下载字幕以便他们能在线阅读。在创建影片组件时，您能将影片和字幕相结合。

自动播放影片的前提是您的字幕必须是srt格式的文档。
若想创建和保存srt格式的字幕，您可以和提供字幕服务的公司合作。
EdX可以和3Play Media公司合作。You Tube也能提供字幕服务。

您上传srt文档时，文本文件会自动生成。学生可以下载srt文档或文本文档（txt）。
若您允许学生下载副本，影片下方会出现下载副本按钮。
学生能够自行选择SubRip文档（.srt文档）或文本文档（.txt）来下载.srt格式或文本文档（txt）格式的副本。

.. image:: ../../../shared/building_and_running_chapters/Images/Video_DownTrans_srt-txt.png
   :width: 500
   :alt: Video status bar showing srt and txt transcript download options

You can also provide transcripts in different formats, such as .pdf, and you
can provide transcripts in different languages. For more information about
these options, see :ref:`Additional Transcripts`.

.. note:: Historically, some courses used .sjson files for video transcripts.
 Use of .sjson files is no longer recommended; however, if transcripts in your
 course use this format, see :ref:`Steps for sjson files`.

.. _Post the Video Online:

*****************************
步骤3 在网上发布影片
*****************************

所有课程应在You Tube上发布。通过默认设置，edX影片播放器能够播放You Tube的影片。

然而，由于You Tube不是在任何地方下均有效的，所以我们建议您将影片也上传到至第三方网站，例如亚马逊S3。
当学生浏览您的课程时，要是You Tube不适用于学生所在地或You Tube无法播放，上传至备用网站的影片能自动播放。
您也能让学生从备用网站上下载影片。
Because YouTube is not available in all locations, however, we recommend that
you also post copies of your videos on a third-party site such as `Amazon S3
<http://aws.amazon.com/s3/>`_. When a learner views a video in your course, if
YouTube is not available in that learner's location or if the YouTube video
does not play, the video on the backup site starts playing automatically. You
can also allow the learners to download the video from the backup site.

在网上公布影片之后，确保您有影片的统一资源定位符（URL）。
若您在多处复制了您的影片，确保您有每一个副本所在位置的统一资源定位符（URL）。 

==================
YouTube
==================

在创建影片后，将影片上传至 `YouTube
<http://www.youtube.com/>`_.

.. note:: You Tube只能上传最长15分钟的影片。
  如果您选择0.75倍播放速度，您必须确定影片片段只有11.25分钟，如此一来才能确保影片全部上传至You Tube。
  You Tube有提供付费机制可以解除这个限制。

==================
其他网站 
==================

您能使用任何备用网站。然而，切记您上传影片的网站可能需要面对网络繁忙的情况。

.. note:: 最终您上传至第三方网站的影片统一资源定位符（URL）必须是mp4, .webm, .mpeg, 或.ogg格式。
（为了确保所有标准浏览器均能播放影片，我们强烈建议您用mp4,或webm.格式）EdX不支持类似Vimeo等网站上的视频。

If you (or your beta testers or learners) encounter an error when you view a
course video, it might be the result of one of these browser-related problems.

* Verify that the browser is up to date. For example, some older versions of
  the Mozilla Firefox browser did not play .mp4 video files, and some older
  versions of the Firefox browser did not play .webm video files. This problem
  does not occur in more recent versions of these browsers.

  For more information, see `Media formats supported by the HTML audio and
  video elements`_.

* Verify that file metadata, particularly the MIME type, is correctly set on
  the host site. Internet Explorer 10 browsers do not play videos if the MIME
  type is not set. For example, make sure that the HTTP header Content-Type
  is set to video/mp4 for an .mp4 file, or to video/webm for a .webm file.

  As an example of how you might set metadata on a video backup site, the
  *Console User Guide* for the Amazon Simple Storage Service provides this
  information about `editing object metadata`_.


.. _Create a Video Component:

********************************
步骤4 创建影片组件
********************************

#. 在新增组件下，点击影片

#. 当出现新的影片组件时，点击编辑。影片编辑者能看见原始码。

   .. image:: ../../../shared/building_and_running_chapters/Images/VideoComponentEditor.png
    :alt: Image of the video component editor
    :width: 500

   您能自行替代默认值。

3. 在显示组件名称栏位，填入您想让学生在鼠标划过页面时显示的提示文字。
   这个文字将成为影片的标题文字。

#. 在默认影片统一资源定位符（URL）栏位，输入影片的统一资源定位符（URL）。
   例如，统一资源定位符（URL）可能类似于以下例子中的一种。

   ::

      http://youtu.be/OEoXaMPEzfM
      http://www.youtube.com/watch?v=OEoXaMPEzfM
      https://s3.amazonaws.com/edx-course-videos/edx-edx101/EDXSPCPJSP13-G030300.mp4
      https://s3.amazonaws.com/edx-videos/edx101/video4.webm

.. note:: 为了确保所有学生均能播放影片，您能在互联网上公布影片的其他版本。
    之后将这些影片的统一资源定位符（URL）添加至下方影片默认统一资源定位符（URL）。
    这些统一资源定位符（URL）不能是You Tube网站的统一资源定位符（URL）。
    想要将统一资源定位符（URL）添加至其他版本中，点击添加其他版本统一资源定位符（URL）。
    与学生们电脑兼容的第一个列明影片将播放。

5. 下一个步骤是默认限时副本，选择一个选项。

   * 若edX已存有您的影片，例如，若您正在播放现有课程中的影片，Studio会自动找到副本并将其与影片连接起来。

     若您想修改副本，点击下载副本及编辑。您能改动影片并通过点击上传新副本完成上传。


   * 若edX没有影片副本，而You Tube有的话，Studio会自动找到You Tube网站上的副本并询问您是否输入副本。
     若要使用You Tube网站上的副本，点击输入You Tube副本。
     （若您想修改You Tube副本，将其输入Studio，接着点击下载副本及编辑。）
     这样，您能修改影片并通过点击上传新副本完成上传。
     

   * 若edX和You Tube都有您的副本，但是edX过期的话，您将收到询问您是否用You Tube副本替代edX副本的消息。
     若同意，点击是，You Tube副本替代edX副本。


   * 若edX和You Tube都没有您的副本，并且您的副本格式是.srt的话，点击上传新副本完成上传。
   

     .. note::

        * 若您的副本使用的是.sjson格式的话，勿用此项设置。
          欲知更多信息，请见 :ref:`Steps for sjson files`.

        * 若您希望提供副本的格式是.pdf的话，勿用此项设置上传副本。
          欲知更多信息，请见 :ref:`Additional Transcripts`.

6. Optionally, click **Advanced** to set more options for the video. For a
   description of each option, see :ref:`Video Advanced Options`.

#. Click **Save.**

.. _Video Advanced Options:

==================
Advanced Options
==================

The following options appear on the **Advanced** tab in the video component.

.. list-table::
    :widths: 30 70

    * - **Component Display Name**
      - The name that you want your learners to see. This is the same as the
        **Display Name** field on the **Basic** tab.
    * - **Default Timed Transcript**
      -  The name of the transcript file that is used in the **Default Timed
         Transcript** field on the **Basic** tab. This field is auto-populated.
         You do not have to change this setting.
    * - **Download Transcript Allowed**
      - Specifies whether you want to allow learners to download the timed
        transcript. If you select **True**, a link to download the
        file appears below the video.

        By default, Studio creates a .txt transcript when you upload an .srt
        transcript. Learners can download the .srt or .txt versions of the
        transcript when you set **Download Transcript Allowed** to **True**. If
        you want to provide the transcript for download in a different format
        as well, such as .pdf, upload a file to Studio by using the **Upload
        Handout** field.

    * - **Downloadable Transcript URL**
      - The URL for a non-.srt version of the transcript file posted on the
        **Files & Uploads** page or on the Internet. Learners see a link to
        download the non-.srt transcript below the video.

        When you add a transcript to this field, only the transcript that you
        add is available for download. The .srt and .txt transcripts become
        unavailable. If you want to provide a downloadable transcript in a
        format other than .srt, we recommend that you upload a handout for
        learners by using the **Upload Handout** field. For more information,
        see :ref:`Additional Transcripts`.

    * - **EdX Video ID**
      - An optional field used only by course teams that are working with
        edX to process and host video files.

    * - **License**
      - Optionally, you can set the license for the video, if you want to
        release the video with a license different from the overall course
        license.

        * Select **All Rights Reserved** to indicate to learners that you own
          the copyright for the video.

        * Select **Creative Commons** to grant others the right to share and
          use the video. You must then select the Creative Commons license
          options to apply.

          The license options that you select control the copyright notice that
          learners see for the video. For more information, see :ref:`Licensing
          a Course`.

    * - **Show Transcript**
      - Specifies whether the transcript plays along with the video by default.
    * - **Transcript Languages**
      - The transcript files for any additional languages. For more
        information, see :ref:`Transcripts in Additional Languages`.
    * - **Upload Handout**
      - Allows you to upload a handout to accompany this video. Your handout
        can be in any format. Learners can download the handout by clicking
        **Download Handout** under the video.
    * - **Video Available on Web Only**
      - If you select **True**, learners are only allowed to play this video
        in a Web browser. If you select **False**, learners can use any
        compatible application to play the video, including Web browsers and
        mobile apps.
    * - **Video Download Allowed**
      - Specifies whether learners can download versions of this video in
        different formats if they cannot use the edX video player or do not
        have access to YouTube. If you select **True**, you must add
        at least one non-YouTube URL in the **Video File URLs** field.
    * - **Video File URLs**
      - The URL or URLs where you posted non-YouTube versions of the video.
        Every URL should end in .mp4, .webm, .mpeg, or .ogg and cannot be a
        YouTube URL. Each learners will be able to view the first listed video
        that is compatible with the his or her computer. To allow learners to
        download these videos, you must set **Video Download Allowed** to
        **True**.

        To help make sure all standard browsers can play your video, we
        **strongly** recommend that you use the .mp4 format.

    * - **Video ID**
      - An optional field used only by course teams that are working with
        edX to process and host video files.
    * - **Video Start Time**
      - The time you want the video to start if you do not want the entire
        video to play. Use HH:MM:SS format. The maximum value is 23:59:59.

        .. note:: Learners who download and play the video in the mobile
         app see the entire video file. Only videos that play in a browser
         start playing at the specified start time.

    * - **Video Stop Time**
      - The time you want the video to stop if you do not want the entire video
        to play. Use HH:MM:SS format. The maximum value is 23:59:59.

        .. note:: Learners who download and play the video in the mobile
         app see the entire video file. Only videos that play in a browser
         stop playing at the specified stop time.

    * - **YouTube IDs**
      - If you have uploaded separate video files to YouTube for different
        speeds of your video (YouTube ID for .75x speed, YouTube ID for 1.25x
        speed, YouTube ID for 1.5x speed), enter the YouTube IDs for these
        videos in these fields. These settings are optional, to support video
        play on older browsers.

.. _Video TOC:

***************************
Video Table of Contents
***************************

You can add a table of contents for your video by adding an .srt transcript
file that contains clickable links to different parts of the video. When your
learners view the video, they can click the **CC** button at the bottom of the
video player to switch between the main transcript for the video and the table
of contents.

To add a table of contents, you work with a third-party service to create
the .srt transcript file. Then, you use the **Transcript Languages** setting
in the video component to associate the .srt file with the video.

.. image:: ../../../shared/building_and_running_chapters/Images/VideoTOC.png
   :alt: Image of a video with a transcript that has links to different parts
    of the video
   :width: 500

#. After you obtain the .srt transcript file that will function as the
   table of contents, open the video component for the video.

#. On the **Advanced** tab, scroll down to **Transcript Languages**, and then
   click **Add**.

#. In the dropdown list that appears, select **Table of Contents**.

   An **Upload** button appears.

#. Click **Upload**, browse to the .srt file for the transcript, and then click
   **Open**.

#. In the **Upload translation** dialog box, click **Upload**.

.. _Additional Transcripts:

**********************
Additional Transcripts
**********************

By default, a .txt file is created when you upload an .srt file, and learners
can download an .srt or .txt transcript when you set **Download Transcript
Allowed** to **True**. The **Download Transcript** button appears below the
video, and learners see the .srt and .txt options when they move the cursor
over the button.

.. image:: ../../../shared/building_and_running_chapters/Images/Video_DownTrans_srt-txt.png
   :width: 500
   :alt: Video status bar showing srt and txt transcript download options

If you want to provide a downloadable transcript in a format such as .pdf along
with the .srt and .txt transcripts, we recommend that you use the **Upload
Handout** field. When you do this, a **Download Handout** button appears to the
right of the **Download Transcript** button, and learners can download the
.srt, .txt, or handout version of the transcript.

.. image:: ../../../shared/building_and_running_chapters/Images/Video_DownTrans_srt-handout.png
   :width: 500
   :alt: Video status bar showing srt, txt, and handout transcript download
    options

To add a downloadable transcript, you use the **Upload Handout** field.

#. Create or obtain your transcript as a .pdf or in another format.
#. In the video component, click the **Advanced** tab.
#. Locate **Upload Handout**, and then click **Upload**.
#. In the **Upload File** dialog box, click **Choose File**.
#. In the dialog box, select the file on your computer, and then click
   **Open**.
#. In the **Upload File** dialog box, click **Upload**.

Before Studio added the **Upload Handout** feature, some courses posted
transcript files on the **Files & Uploads** page or on the Internet, and then
added a link to those files in the video component. **We no longer recommend
this method.**  When you use this method, the **Download Transcript** button
appears, but only the transcript that you add is available for download. The
.srt and .txt transcripts become unavailable.

.. image:: ../../../shared/building_and_running_chapters/Images/Video_DownTrans_other.png
   :width: 500
   :alt: Video status bar showing Download Transcript button without srt and
    txt options

If you want to use this method, you can post your transcript online, and then
add the URL to the transcript in the **Downloadable Transcript URL** field.
However, bear in mind that learners will not be able to download .srt or .txt
transcripts.

.. _Transcripts in Additional Languages:

====================================
Transcripts in Additional Languages
====================================

You can provide transcripts for your video in other languages. To do this,
you work with a third-party service to obtain an .srt transcript file for
each language, and then associate the .srt file with the video in Studio.

#. After you obtain the .srt files for additional languages, open the
   video component for the video.

#. On the **Advanced** tab, scroll down to **Transcript Languages**, and then
   click **Add**.

#. In the drop-down list that appears, select the language for the transcript
   that you want to add.

   An **Upload** button appears below the language.

#. Click **Upload**, browse to the .srt file for the language that you want,
   and then click **Open**.

#. In the **Upload translation** dialog box, click **Upload**.

#. Repeat steps 2 - 5 for any additional languages.

.. note:: Make sure that all your transcript file names are unique to each
 video and language. If you use the same transcript name in more than one video
 component, the same transcript will play for each video. To avoid this
 problem, you could name your foreign language transcript files according to
 the video's file name and the transcript language.

 For example, you have two videos, named video1.mp4 and video2.mp4. Each video
 has a Russian transcript and a Spanish transcript. You can name the
 transcripts for the first video video1_RU.srt and video1_ES.srt, and name the
 transcripts for the second video video2_RU.srt and video2_ES.srt.

When your learners view the video, they can click the **CC** button at the
bottom of the video player to select a language.

.. image:: ../../../shared/building_and_running_chapters/Images/Video_LanguageTranscripts_LMS.png
   :alt: Video playing with language options visible

.. _Steps for sjson files:

**********************
Steps for .sjson Files
**********************

If your course uses .sjson files, you upload the .sjson file for the video
to the **Files & Uploads** page, and then specify the name of the .sjson file
in the video component.

.. note:: Only older courses that have used .sjson files in the past should use
 .sjson files. All new courses should use .srt files.

#. Obtain the .sjson file from a media company such as 3Play.
#. Change the name of the .sjson file to use the following format.

   ``subs_{video filename}.srt.sjson``

   For example, if the name of your video is **Lecture1a**, the name of your
   .sjson file must be **subs_Lecture1a.srt.sjson**.

#. Upload the .sjson file for your video to the **Files & Uploads** page.
#. Create a new video component.
#. On the **Basic** tab, enter the name that you want learners to see in the
   **Component Display Name** field.
#. In the **Video URL** field, enter the URL of the video. For example, the URL
   may resemble one of the following.

   ::

      http://youtu.be/OEoXaMPEzfM
      http://www.youtube.com/watch?v=OEoXaMPEzfM
      https://s3.amazonaws.com/edx-course-videos/edx-edx101/EDXSPCPJSP13-G030300.mp4

#. Click the **Advanced** tab.
#. In the **Default Timed Transcript** field, enter the file name of your
   video. Do not include `subs_` or `.sjson`. For the example in step 2, you
   would only enter **Lecture1a**.
#. Set the other options that you want.
#. Click **Save**.

.. _Creating Videos: https://courses.edx.org/courses/edX/edX101/2014/courseware/c2a1714627a945afaceabdfb651088cf/9dd6e5fdf64b49a89feac208ab544760/

.. _edX101 Overview of Creating an edX Course: https://www.edx.org/node/5496#.VH8p51fF_FA
.. _Media formats supported by the HTML audio and video elements: https://developer.mozilla.org/en-US/docs/Web/HTML/Supported_media_formats#MP4_H.264_(AAC_or_MP3)
.. _editing object metadata: http://docs.aws.amazon.com/AmazonS3/latest/UG/EditingtheMetadataofanObject.html
