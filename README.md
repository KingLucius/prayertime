# prayertime
python library for calculating prayertimes and qibla direction.


## Example



```python

pt = Prayertime(31.2599, 30.0599, 2, 2010, 8, 6, Calendar.EgyptianGeneralAuthorityOfSurvey, Mazhab.Default, Season.Summer, TimeFormat.24H)
print(pt.get_qibla())
pt.calculate()
pt.report()
    
```

## API 
- To initialize prayertime object, you need to pass`longitude`, `latitude`, `zone`, `year`, `month`, `day`, `calendar`, `mazhab` , `season`, `timeformat`

- Calendar (UmmAlQuraUniv, EgyptianGeneralAuthorityOfSurvey UnivOfIslamicSciencesKarachi, IslamicSocietyOfNorthAmerica)
- Mazhab (Default, Hanafi)
- Seasons (Summer, Winter)
- TimeFormat (H12, H24)
