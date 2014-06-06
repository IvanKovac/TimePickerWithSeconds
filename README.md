TimePickerWithSeconds
=====================

Android TimePicker widget with seconds field included together with hours and minutes. This is extension of existing Androids TimePicker widget. It is developed above that widget.

![alt tag](https://raw.github.com/IvanKovac/TimePickerWithSeconds/master/Screenshot_2014-03-03-19-55-49.png)



Aplication
------
It is under the root dir : TimePickerWithSeconds.apk

Quick Setup
------

This is Android library project. To use it within your application follow these steps:

1. Download the project to your workspace
2. Import project into Eclipse
3. Right click on YOUR project - > Properties -> Android 
   Under the library choose "Add" and add TimePickerWithSeconds project
4. Show the Picker with:
   
``` java
MyTimePickerDialog mTimePicker = new MyTimePickerDialog(this, new MyTimePickerDialog.OnTimeSetListener() {

			@Override
			public void onTimeSet(TimePicker view, int hourOfDay, int minute, int seconds) {
				// TODO Auto-generated method stub
				/*time.setText(getString(R.string.time) + String.format("%02d", hourOfDay)+
						":" + String.format("%02d", minute) + 
						":" + String.format("%02d", seconds));	*/			
			}
		}, now.get(Calendar.HOUR_OF_DAY), now.get(Calendar.MINUTE), now.get(Calendar.SECOND), true);
		mTimePicker.show();
```


Enjoy!

Licence
------
Feel free to use and change this code and include it in any of the projects you wish. There is no guarantee of any kind.
