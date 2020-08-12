# Next Steps

Hosting this site in production would require a few additional steps. Notably, it's likely that you would use WhiteNoise on the server for your static files, however WhiteNoise explicitly does not support media files. The common practice is to use django-storages for this purpose and connect to something like S3.

What else? You probably want to put restrictions around the image size which can be done initially in the models.py file or with CSS. Perhaps you want to add edit and delete options as well for the Post. And you'll likely want a thumbnail version of the images too which can be done with sorl-thumbnail.
