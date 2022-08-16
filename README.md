# Purpose

An application which displays an image collected from the NASA API at [this endpoint](https://api.nasa.gov/planetary/apod).

# Persisted settings

We use the UWP feature `LocalSettings` to create persistent data. We persist data by giving the user the option of not displaying today's astronomy picture on startup, in case they've already seen it or don't want to use up one of their 50 downloads per day (the NASA endpoint has a limit of 50 downloads per day). We save:

- today's date,
- the startup setting,
- the count of images already downloaded today
- the setting that limits the range of dates

# References

- https://docs.microsoft.com/en-us/learn/modules/build-internet-connected-windows10-app
