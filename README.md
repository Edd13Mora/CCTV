# CCTV
Close-Circuit Telegram Vision revolutionizes location tracking with its open-source design and Telegram API integration. Offering precise tracking within 50-100 meters, users can monitor others in real-time for logistics or safety, redefining how we navigate our surroundings

Usage example:
--------------
1. Installation 
```
git clone https://github.com/IvanGlinkin/CCTV.git
cd CCTV
pip install -r requirements.txt
```

2. Registering Telegram creds
```
visit https://my.telegram.org/auth web-site
input your phone number
input the confirmation/login code
follow "API development tools" link
register the application
get App's api_id, api_hash, title and name
```

3. Setting up Telegram creds
```
nano ./backend/telegram_creds.py
  phone_number = 'your_phone_number' // put your phone number 
  telegram_name = 'api_name' // put your API name from the step 2
  telegram_api_id = 'api_id' // put your API ID from the step 2
  telegram_api_hash = 'api_hash' // put your API Hash from the step 2
```

4. Launch
```
nano general_settings.py // set the location and radius
python3 start.py
```

5. Read the data by opening ./reports-html/_combined_data.html

Help message:
-------------
```

 ██████╗██╗      ██████╗ ███████╗███████╗     ██████╗██╗██████╗  ██████╗██╗   ██╗██╗████████╗                      
██╔════╝██║     ██╔═══██╗██╔════╝██╔════╝    ██╔════╝██║██╔══██╗██╔════╝██║   ██║██║╚══██╔══╝                      
██║     ██║     ██║   ██║███████╗█████╗█████╗██║     ██║██████╔╝██║     ██║   ██║██║   ██║                         
██║     ██║     ██║   ██║╚════██║██╔══╝╚════╝██║     ██║██╔══██╗██║     ██║   ██║██║   ██║                         
╚██████╗███████╗╚██████╔╝███████║███████╗    ╚██████╗██║██║  ██║╚██████╗╚██████╔╝██║   ██║                         
 ╚═════╝╚══════╝ ╚═════╝ ╚══════╝╚══════╝     ╚═════╝╚═╝╚═╝  ╚═╝ ╚═════╝ ╚═════╝ ╚═╝   ╚═╝                         
                                                                                                                   
████████╗███████╗██╗     ███████╗ ██████╗ ██████╗  █████╗ ███╗   ███╗    ██╗   ██╗██╗███████╗██╗ ██████╗ ███╗   ██╗
╚══██╔══╝██╔════╝██║     ██╔════╝██╔════╝ ██╔══██╗██╔══██╗████╗ ████║    ██║   ██║██║██╔════╝██║██╔═══██╗████╗  ██║
   ██║   █████╗  ██║     █████╗  ██║  ███╗██████╔╝███████║██╔████╔██║    ██║   ██║██║███████╗██║██║   ██║██╔██╗ ██║
   ██║   ██╔══╝  ██║     ██╔══╝  ██║   ██║██╔══██╗██╔══██║██║╚██╔╝██║    ╚██╗ ██╔╝██║╚════██║██║██║   ██║██║╚██╗██║
   ██║   ███████╗███████╗███████╗╚██████╔╝██║  ██║██║  ██║██║ ╚═╝ ██║     ╚████╔╝ ██║███████║██║╚██████╔╝██║ ╚████║
   ╚═╝   ╚══════╝╚══════╝╚══════╝ ╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝     ╚═╝      ╚═══╝  ╚═╝╚══════╝╚═╝ ╚═════╝ ╚═╝  ╚═══╝

usage: start.py [-h] [-lat LATITUDE] [-long LONGITUDE] [-m METERS] [-t TIMESLEEP] [-tn TELEGRAM_NAME]
                [-ti TELEGRAM_API_ID] [-th TELEGRAM_API_HASH]

Custom settings for script launch

optional arguments:
  -h, --help            show this help message and exit
  -lat LATITUDE, --latitude LATITUDE
                        Latitude setting
  -long LONGITUDE, --longitude LONGITUDE
                        Longitude setting
  -m METERS, --meters METERS
                        Meters setting
  -t TIMESLEEP, --timesleep TIMESLEEP
                        Timesleep setting
  -tn TELEGRAM_NAME, --telegram_name TELEGRAM_NAME
                        Telegram username
  -ti TELEGRAM_API_ID, --telegram_api_id TELEGRAM_API_ID
                        Telegram API ID
  -th TELEGRAM_API_HASH, --telegram_api_hash TELEGRAM_API_HASH
                        Telegram API hash
```

Video example:
--------------
![https://github.com/IvanGlinkin/media_support/blob/main/CCTV_Github.mp4](https://github.com/IvanGlinkin/media_support/blob/main/CCTV_Github.mp4?raw=true)

Screenshots:
------------
![](https://raw.githubusercontent.com/IvanGlinkin/media_support/main/CCTV1.png)
![](https://raw.githubusercontent.com/IvanGlinkin/media_support/main/CCTV2.png)
![](https://raw.githubusercontent.com/IvanGlinkin/media_support/main/CCTV4.png)
