# Home Assistant NFL Card
A Home Assistant frontend custom card for the [ha-nhl](https://github.com/simplysynced/ha-nhl) integration.  This was originaly made by @D34DC3N73R [ha-nfl-card](https://github.com/D34DC3N73R/ha-nfl-card)

#### &nbsp;&nbsp;&nbsp;PREGAME

![pregame](NEED IMAGE)

#### &nbsp;&nbsp;&nbsp;IN GAME

![ingame](NEED IMAGE)

#### &nbsp;&nbsp;&nbsp;POSTGAME

![postgame](NEED IMAGE)

#### &nbsp;&nbsp;&nbsp;BYE

![bye](NEED IMAGE))


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
| `outline` | Outline team colors (helpful w/ dark themes) |`false` | No |  `true` `false` |
| `outline_color` | Specifies outline color. | `white` | No |  CSS color or hex value  |

## Examples
```
type: 'custom:nhl-card'
entity: sensor.nhl
outline: true
outline_color: deeppink
```
![example](NEED IMAGE)


```
type: 'custom:nhl-card'
entity: sensor.nhl
outline: true
outline_color: '#ffe500'
```
![example2](NEED IMAGE)

## Minimal Required Configuration
```
type: 'custom:nhl-card'
entity: sensor.nhl
```
Where `sensor.nhl` is the sensor name from the [ha-nhl](https://github.com/simplysynced/ha-nhl) integration.
