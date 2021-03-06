Timepicker Plugin for jQuery
========================

[<img src="http://jonthornton.github.com/jquery-timepicker/lib/screenshot.png" alt="timepicker screenshot" />](http://jonthornton.github.com/jquery-timepicker)

[See a demo and examples here](http://jonthornton.github.com/jquery-timepicker)

jquery.timepicker is a timepicker plugin for jQuery inspired by Google Calendar. It supports both mouse and keyboard navigation.

Requirements
------------
* [jQuery](http://jquery.com/) (>= 1.6 recommended; jquery-timepicker has not been tested on 1.5)

Usage
-----

```javascript
$('.some-time-inputs').timepicker(options);
```

```options``` is an optional javascript object with parameters explained below.

Options
-------

- **className**  
A class name to apply to the HTML element that contains the timepicker dropdown.  
*default: null*

- **minTime**  
The time that should appear first in the dropdown list. 
*default: 12:00am*

- **maxTime**
The time that should appear last in the dropdown list. Can be used to limit the range of time options.
*default: 24 hours after minTime*

- **showDuration**  
Shows the relative time for each item in the dropdown. ```minTime``` or ```durationTime``` must be set.  
*default: false*

- **durationTime**  
The time against which ```showDuration``` will compute relative times.  
*default: minTime*

- **step**  
The amount of time, in minutes, between each item in the dropdown.  
*default: 30*

- **timeFormat**  
How times should be displayed in the list and input element. Uses [PHP's date() formatting syntax](http://php.net/manual/en/function.date.php).  
*default: 'g:ia'*

- **scrollDefaultNow**  
If no time value is selected, set the dropdown scroll position to show the current time.  
*default: false*

- **onSelect**  
A function to call after the user selects a time from the dropdown. Function will be with no arguments and ```this``` set to the input element. jquery-timepicker will also trigger the onChange event for the input element.  
*default: null*


- - -

This software is made available under the open source MIT License. &copy; 2012 [Jon Thornton](http://www.jonthornton.com), contributions from [Anthony Fojas](https://github.com/fojas), [Vince Mi](https://github.com/vinc3m1), [Nikita Korotaev](https://github.com/websirnik), [Spoon88](https://github.com/Spoon88), [elarkin](https://github.com/elarkin)
