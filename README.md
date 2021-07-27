<div align="center">

<img src="https://github.com/speeduino/wiki.js/raw/master/img/Speeduino%20logo_med.png" alt="Speeduino" width="600" />
 
[![Chat on Slack](https://img.shields.io/badge/slack-speeduino-CC2B5E.svg?style=flat&logo=slack)](https://speeduino.com/home/community/slack)

##### A low cost, DIY friendly Engine Management System (ECU) based on the Arduino framework
</div>


## Speeduino
The Speeduino project is a flexible, fully featured Engine Management Systems (EMS aka ECU) based on the low cost and open source Arduino platform. It provides the hardware, firmware and software components that make up an engine management system, all provided under open licenses. With over 1000 installations, Speeduino has matured into a product that meets the needs of the hobbyist and enthusiast community without driving prices to the levels of traditional aftermarket ECUs.

## Overview
This repositiory contains official and user contributed tune files that can then be downloaded through [SpeedyLoader](https://github.com/speeduino/SpeedyLoader)

## How do I contribute a tune?
This library contains both official tunes as well as user contributed ones. If you'd like to contribute your tune, a Pull Request can be submitted against this repository to get it added. 

Please note that all tunes submitted are released under the [Creative Commons CC BY-NC 4.0 license](https://creativecommons.org/licenses/by-nc/4.0/). 

When adding your tune, 2 main steps are needed:

1. Your tune file should be placed in the relevant manufacturer folder (Eg "Mazda", "BMW" etc). If the manufacturer for your tune does not exist already, you should create this folder
2. You will need to add an entry into the bottom of the `index.json` file with the details of your tune. A sample entry is below:
```
{
    "id": "3",
    "displayName": "Miata / MX5 96-97 PNP",
    "make": "Mazda",
    "firmware": 201909,
    "provider": "Speeduino",
    "type": "Stock",
    "board": "Miata NA8 PNP",
    "description": "Tune for use with the Speeduino PNP units on 1996-1997 NA8 Miata + MX5",
    "filename": "NA8%20PNP%20base%20tune.msq"
},
```

### Field List:

* id: This should be the next number from the previous last entry in the file
* displayName: A brief description of the engine / car your tune is for. If it is a non-stock tune then a very brief description of the modifications should be added. Eg: `Miata / MX5 96-97 PNP with Turbo`
* make: The manufacturer of the car/engine the tune is for. **Must match the folder name that the tune file has been placed in (case sensitive)**
* firmware: The firmware version that the tune was created with
* provider: A username that will be shown in SpeedyLoader for who authored the tune
* type: Either `Stock` or `Modified` depending on whether the tune is for a stock engine setup or a modified one
* board: The hardware design that the tune was developed on (Eg v0.4, NA6 PNP etc)
* description: A longer description of the tune. If it is for a modified engine, please describe in detail the modifications you've made
* filename: The filename of the tune

## License
All tunes are provided under the [Creative Commons CC BY-NC 4.0 license](https://creativecommons.org/licenses/by-nc/4.0/). 

## Support
In addition the manual referenced above, Speeduino has a large and very vibrant community of people to help out with your setup or any questions you might add. 

* [Speeduino Manual](https://wiki.speeduino.com)
* [Speeduino Forum](https://speeduino.com/forum) 
* [Slack](https://speeduino.com/home/community/slack)
* [Facebook](https://www.facebook.com/groups/191918764521976/)

## Contributors

This project exists thanks to all the people who contribute, both in terms of code and testing provided. If you'd like to get involved, please have a read through [Contributing](contributing.md) and then jump on Slack to discuss things further
