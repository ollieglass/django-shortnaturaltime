django-shortnaturaltime
=

For datetime values, returns a string representing how long ago it was in a very short, humanized form.

Based on Django's humanize.[naturaltime filter](https://docs.djangoproject.com/en/dev/ref/contrib/humanize/) and Instagram's abbreviation style.

Examples
-

Examples (when ‘now’ is 17 Feb 2007 16:30:00):

* 17 Feb 2007 16:30:00 becomes `now`
* 17 Feb 2007 16:29:31 becomes `29s`
* 17 Feb 2007 16:29:00 becomes `1m`
* 17 Feb 2007 16:25:35 becomes `4m`
* 17 Feb 2007 15:30:29 becomes `1h`
* 17 Feb 2007 13:31:29 becomes `2h`
* 16 Feb 2007 16:30:00 becomes `1d`
* 15 Feb 2007 16:30:00 becomes `2d`
* 17 Jan 2007 16:30:00 becomes `1m`
* 17 Feb 2006 16:30:00 becomes `1y`
* 16 Feb 2006 16:30:00 becomes `1y 1d`
* 17 Jan 2006 16:30:00 becomes `1y 1m`

Installation and usage
-
* Create a folder in your Django app called 'templatetags'
* Add an empty __init__.py file and the shortnaturaltime.py file
* In templates, use `{{ time_value|shortnaturaltime }}` to render the short natural time.

