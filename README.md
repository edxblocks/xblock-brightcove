Brightcove Video Player XBlock
------------------------------

This XBlock provides a HTML5 video player for Brightcove.

Screenshot below shows the Brightcove Video Player XBlock rendered
inside the edX LMS.

![Student view](https://raw.githubusercontent.com/edx-solutions/xblock-brightcove/0f08b1f3c0dbb47d6b698980208871a7055f7e9f/doc/img/student-view.png)

Installation
------------

Install the requirements into the python virtual environment of your
`edx-platform` installation.

```bash
$ pip install -r requirements.txt
```

Enabling in Studio
------------------

You can enable the Brightcove Video Player XBlock in studio through
the advanced settings.

1. From the main page of a specific course, navigate to `Settings ->
   Advanced Settings` from the top menu.
2. Check for the `advanced_modules` policy key, and add
   `"brightcove-video"` to the policy value list.
3. Click the "Save changes" button.

Usage
-----

After adding a Brightcove Video XBlock to a course, there are two
settings you should set in the studio edit view: _Brightcove video
URL_ and _Brightcove API key_.

Note: You will need to create a free trial account on the Brightcove
website to do get them. See the 
[Brightcove documentation](http://support.brightcove.com/en/video-cloud/docs/managing-media-api-tokens#get) 
to learn how to get your API key.

![Edit view](https://raw.githubusercontent.com/edx-solutions/xblock-brightcove/0f08b1f3c0dbb47d6b698980208871a7055f7e9f/doc/img/edit-view.png)

The video URL is a short URL pointing to your video that should look
something like `http://bcove.me/q5thswyv`.

The API key is needed in order to automatically pull additional video
information (such as the video name) from the Brightcove HTTP API.

The API key can be found in the Brightcove admin under `Account
Settings -> API Management`. Use the `read` token as the API key.

License
-------

The Brightcove XBlock is available under the GNU Affero General
Public License (AGPLv3).
