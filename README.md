# Custom-Django-Select-Time-Widget

modifed from 
https://www.djangosnippets.org/snippets/1202/
https://bradmontgomery.net/blog/selecttimewidget-a-custom-django-widget/
made seconds optional and fixed some bugs.

Similar to the SelectDateWidget located in django.forms.extras.widgets. Works with Times instead of Dates.

The SelectTimeWidget supports both 24-hr and 12-hr formats, and flexible time increments for hours, minutes and seconds.

###### Specify a basic 24-hr time Widget (the default)
t = forms.TimeField(widget=SelectTimeWidget())

###### Force minutes and seconds to be displayed in increments of 10
t = forms.TimeField(widget=SelectTimeWidget(minute_step=10, second_step=10))

###### Use a 12-hr time format, which will display a 4th select element containing a.m. and p.m. options)
t = forms.TimeField(widget=SelectTimeWidget(twelve_hr=True))
