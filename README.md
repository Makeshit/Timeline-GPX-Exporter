# Timeline-GPX-Exporter
Convert Google Timeline JSON exported from an Android device to daily GPX log files

I created this because I needed an easy way to find time stamps from the last year of my raw timeline data, a function that irritatingly no longer exists since timeline went device only with the now very limited Android Maps Timeline interface.

1. Export timeline data from your Android device. 

To do this, on your Android device go to **settings > Location > Timeline > Export Timeline data**.  

2. Place the exported Timeline.json file into the same folder as Timeline-GPX-Exporter.py

3. Run Timeline-GPX-Exporter.py script. Daily GPX logs with be generated in ./GPX_Output with the format YYYY-MM-DD.gpx. 

4. Open the GPX logs in your veiewer of choice. 
GPXsee is a gppd option, however you may need to disable Elimiate GPS outliers from settings > Data > Filtering 
and disable pause dectection from settings > Data > Pause Detection.

Example: Place both Timeline-GPX-Exporter.py and Timeline.json in C:/Timeline

         Open command prompt
         >cd C:\Timeline
         >python Timeline-GPX-Exporter.py

The GPX log files produced are not perfect, some less forgiving viewers might reject them. However it did what I needed it to do perfectly, so as far as I'm concerned it's certified good enough. If it's good enough for you too, then great, you're welcome. If it's not, well too bad, I have what I needed from it and you're more than welcome to take it and adapt it to suit your needs.
