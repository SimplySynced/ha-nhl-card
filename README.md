# Home Assistant NHL Card
A Home Assistant frontend custom card for the [ha-nhl](https://github.com/simplysynced/ha-nhl) integration.  This was originaly made by @D34DC3N73R for the NFL and can be found here [ha-nfl-card](https://github.com/D34DC3N73R/ha-nfl-card)

#### &nbsp;&nbsp;&nbsp;PREGAME

![nhl_card_pre](https://user-images.githubusercontent.com/22181015/147371178-a3306e2a-5dff-481c-a436-93534c0eae78.jpg)

#### &nbsp;&nbsp;&nbsp;IN GAME

![nhl_card_in](https://user-images.githubusercontent.com/22181015/147807404-884aed3d-91de-4a47-a790-8fe777cab06b.jpg)

#### &nbsp;&nbsp;&nbsp;POSTGAME

![nhl_card_post](https://user-images.githubusercontent.com/22181015/147807415-42fdf195-a9f2-4ef8-99f8-09490170db64.jpg)

#### &nbsp;&nbsp;&nbsp;POSTPONED

![nhl_card_postponed](https://user-images.githubusercontent.com/22181015/147341318-8afa9a7c-8f13-484d-8502-0328c262288b.jpg)



## HACS Installation
- In the HACS UI, click the 3 dots in the upper right
- Click 'Add Custom Repository'
- Fill in the repo url https://github.com/SimplySynced/ha-nhl-card and choose 'Lovelace' category.
- install the custom card
- Add the following to your resources
```
url: /hacsfiles/ha-nhl-card/ha-nhl-card.js
type: module
```

## Manual Installation
- Download [ha-nhl-card.js](https://raw.githubusercontent.com/SimplySynced/ha-nhl-card/main/dist/ha-nhl-card.js)
- Copy to www/community/ha-nhl-card/ (make the ha-nhl-card directory)
- Add the following to your resources
```
url: /hacsfiles/ha-nhl-card/ha-nhl-card.js
type: module
```

## Options
| Name | Description | Default | Required |  Values |
| --- | --- | --- | --- | --- |
| `entity` | Name of ha-nhl sensor | `sensor.nhl` | Yes  | Valid sensor |

## Minimal Required Configuration
```
type: 'custom:nhl-card'
entity: sensor.nhl
```
Where `sensor.nhl` is the sensor name from the [ha-nhl](https://github.com/simplysynced/ha-nhl) integration.