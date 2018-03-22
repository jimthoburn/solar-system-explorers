# Solar System Explorers
An example of how to use the people API from solarsystem.nasa.gov

https://jimthoburn.github.io/solar-system-explorers/

## Example requests for the People API on solarsystem.nasa.gov

### All people
```https://solarsystem.nasa.gov/api/v1/site_staffs/?category=4```

### Featured people
```https://solarsystem.nasa.gov/api/v1/site_staffs/?category=4:134```

### Tributes
```https://solarsystem.nasa.gov/api/v1/site_staffs/?category=4:147```

### People tagged with “Saturn”
```https://solarsystem.nasa.gov/api/v1/site_staffs/?category=4&tags=saturn```

### Limit to 20 people per page
```https://solarsystem.nasa.gov/api/v1/site_staffs/?category=4&per_page=20&page=0```

### Get the next page
```https://solarsystem.nasa.gov/api/v1/site_staffs/?category=4&per_page=20&page=1```

### Order the data by name, ascending
```https://solarsystem.nasa.gov/api/v1/site_staffs/?category=4&order=name+asc```

### Order the data by name, descending
```https://solarsystem.nasa.gov/api/v1/site_staffs/?category=4&order=name+desc```
