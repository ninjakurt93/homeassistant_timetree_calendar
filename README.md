# homeassistant_timetree_calendar 

Create your Token here: [Create token](https://timetreeapp.com/developers/personal_access_tokens)

After that, replace the 'YOURAPIKEY' in Calendar.py with your Token

For Changing the TimeZone, start Date, search for 
`self._entities = timetree_object.get_upcoming_events(self._calendar.id, 'Europe/Berlin', 7).data`
in Calendar.py and change it accordingly

Create a Folder with the name: `timetree` in `Config/custom_components`
paste the files into it.

Dont forget to add the following to your Configuration.yaml:

```yaml
calendar:
  - platform: timetree
```

Credits: 
TimeTree SDK (https://pypi.org/project/timetree-sdk/) has been created by Shoya Shiraki under the MIT License
