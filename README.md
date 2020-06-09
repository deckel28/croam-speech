**Open Speech Recording** is a small web application to collect short snippets
of speech, and upload them to cloud storage. It's designed to help gather open
speech data sets to train machine learning systems.

It's based around a small Flask app that will run on Google App Engine. This serves up a client-side Javascript app that prompts for a series of words, records the audio, and then POSTs the results back to the server.

## Running

To get started, you'll need to edit app.yaml to point to your own storage bucket and update the session key. If you have the Google Cloud SDK set up, to deploy it to an appspot instance, run this:

```
gcloud app deploy
```

