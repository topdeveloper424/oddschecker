# Oddschecker

Foobar is a Python library for matching odds from "https://www.oddschecker.com/football#bumper-coupon".

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.

## UI

https://user-images.githubusercontent.com/40516126/97140253-f02daf80-173a-11eb-93ab-798dac04031f.png


## Algorithm

1. Goto Oddschecker website https://www.oddschecker.com/football#bumper-coupon In the above FootballÆ bumper-coupon site Record the followings to Excel

2. Remove the teams with draw odd < 3.6 (adjustable) 

3. Home oddor Away odd must be within the following range(adjustable) 1.5 (adjustable)<= Home odd or Away odd <= 1.75 (adjustable)    Remove the teams with both home oddand away odd not in this range. 

4. For the remaining teams, do the following calculation Abs(Home add-Away odd) must be>3.3 (adjustable) i.e. Home odd-Away odd >3.3 or Away odd-Home odd >3.3   Remove the teams with this odd difference value =< 3.3 

5. Sort the remaining teams with this odds difference value in decending order E,g: the final table should be like the attached one.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
