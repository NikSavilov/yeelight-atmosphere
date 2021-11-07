# yeelight-atmosphere
The package allows you to control yeelight smart bulbs, 
changes color according to the color scheme of the image on the screen. 

##  Installation 

    pip install yeelight-atmosphere

## Usage:

    cd yeelight-atmosphere
    python main.py

Use --choose flag to force choose a bulb by network scanning 
otherwise previous bulb if exists will be used. 

    python main.py --choose

To choose a part of screen to parse for a color use --strategy flag. Full screen needs more CPU.
- Center area of screen = 0
- Top and bottom borders = 1
- Full screen = 2 
  
    
    python main.py --strategy 0


To modify delay of changing color use --dalay (seconds). The less the smoother.

    python main.py --delay 0.3


# Dependencies:
- Pillow
- sqlalchemy
- yeelight
- colorthief