# Picture Organizer

Picture organizer looks at all the pictures in a directory, creates directories based on date and moves the pictures into those directories. You can rename directories to make things more discoverable as long as you keep the YYYY-MM-DD at the beginning of the directory name, it will still use that directory for categorization.

Dates are based off of the EXIF data, unless none exists, in which case it falls back to the file creation date.

To run it:

```sh
bundle exec organizer organize
```

It defaults to organizing the directory `~/Dropbox (Personal)/Camera Uploads`, you may optionally pass a directory on the command line:

```sh
bundle exec organizer organize /my/fancy/picture/directory
```
