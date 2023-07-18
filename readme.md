# Screenshot

## Alien
### Blocks
![Alien](/Alien.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Spaceship"
          }
        ]
      },
      {
        "targetIndex": 1,
        "blocks": [
          {
            "opcode": "event_whenkeypressed",
            "topLevel":true,
            "fields": { "KEY_OPTION": ["*", null] }
          },
          {
            "opcode": "sound_play",
            "inputs": { "SOUND_MENU": [1, "*"] }
          },
          {
            "opcode": "sound_sounds_menu",
            "fields": { "SOUND_MENU": ["*", null] }
          },
          {
            "opcode": "event_whenflagclicked",
            "topLevel": true
          },
          {
            "opcode": "looks_say",
            "inputs": { "MESSAGE": [1, [10, "*"]] }
          }
        ]
      }
    ]
  }
 ```

## Bear
### Blocks
![Bear](/Bear.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Woods"
          }
        ]
      },
      {
        "targetIndex": 1,
        "blocks": [
          {
            "opcode": "event_whenflagclicked",
            "topLevel":true
          },
          {
            "opcode": "control_repeat",
            "inputs": { "TIMES": [1, [6, "*"]], "SUBSTACK": [2, "*"] }
          },
          {
            "opcode": "motion_movesteps",
            "inputs": { "STEPS": [1, [4, "*"]] }
          },
          {
            "opcode": "looks_nextcostume"
          }
        ]
      }
    ]
  }
 ```


 ## BearCat
### Blocks
![BearCat](/BearCat.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Woods"
          }
        ]
      },
      {
        "targetIndex": 1,
        "blocks": [
          {
            "opcode": "event_whenflagclicked",
            "topLevel": true
          },
          {
            "opcode": "motion_gotoxy",
            "inputs": { "X": [1, [4, "*"]], "Y": [1, [4, "*"]] }
          },
          {
            "opcode": "looks_setsizeto",
            "inputs": { "SIZE": [1, [4, "*"]] }
          },
          {
            "opcode": "looks_switchcostumeto",
            "inputs": { "COSTUME": [1, "*"] }
          },
          {
            "opcode": "looks_costume",
            "fields": { "COSTUME": ["*", null] }
          },
          {
            "opcode": "sound_play",
            "inputs": { "SOUND_MENU": [1, "*"] }
          },
          {
            "opcode": "sound_sounds_menu",
            "fields": { "SOUND_MENU": ["*", null] }
          },
          {
            "opcode": "procedures_call"
          },
          {
            "opcode": "looks_switchcostumeto",
            "inputs": { "COSTUME": [1, "*"] }
          },
          {
            "opcode": "looks_costume",
            "fields": { "COSTUME": ["*", null] }
          },
          {
            "opcode": "procedures_definition",
            "topLevel": true,
            "inputs": { "custom_block": [1, "*"] }
          },
          {
            "opcode": "procedures_prototype"
          },
          {
            "opcode": "control_repeat"
          },
          {
            "opcode": "argument_reporter_string_number",
            "fields": { "VALUE": ["*", null] }
          },
          {
            "opcode": "looks_nextcostume"
          },
          {
            "opcode": "control_wait",
            "inputs": { "DURATION": [3, "*", [5, "*"]] }
          },
          {
            "opcode": "argument_reporter_string_number",
            "fields": { "VALUE": ["*", null] }
          }
        ]
      }
    ]
  }
 ```



  ## Blackboard
### Blocks
![Blackboard](/Blackboard.jpg)
![Blackboard1](/Blackboard1.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Chalkboard"
          }
        ]
      },
      {
        "targetIndex": 1,
        "blocks": [
          {
            "opcode": "event_whenflagclicked",
            "topLevel": true
          },
          {
            "opcode": "looks_sayforsecs",
            "inputs": {
              "MESSAGE": [1, [10, "*"]],
              "SECS": [1, [4, "*"]]
            }
          }
        ]
      },
      {
        "targetIndex": 2,
        "blocks": [
        ]
      },
      {
        "targetIndex": 3,
        "blocks": [
            {
              "opcode": "event_whenflagclicked",
              "topLevel": true
            },
            {
              "opcode": "looks_changesizeby",
              "inputs": { "CHANGE": [1, [4, "*"]] }
            }
        ]
      }
    ]
  }
 ```


  ## Car
### Blocks
![Car](/Car.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Urban"
          }
        ]
      },
      {
        "targetIndex": 1,
        "blocks": [
          {
            "opcode": "event_whenkeypressed",
            "topLevel": true
          },
          {
            "opcode": "sound_playuntildone",
            "inputs": { "SOUND_MENU": [1, "*"] }
          },
          {
            "opcode": "sound_sounds_menu",
            "fields": { "SOUND_MENU": ["*", null] }
          }
        ]
      }
    ]
  }
 ```


   ## Concert
### Blocks
![Concert](/Concert.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Concert"
          }
        ]
      },
      {
        "targetIndex": 1,
        "blocks": [],
        "name":"Drum-cymbal"
      },
      {
        "targetIndex": 2,
        "blocks": [],
        "name": "Drums Tabla"
      },
      {
        "targetIndex": 3,
        "blocks": [],
        "name": "Drums Conga"
      },
      {
        "targetIndex": 4,
        "blocks": [],
        "name": "Prince"
      }
    ]
  }
 ```


  ## Dance
### Blocks
![Dance](/Dance.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Concert"
          }
        ]
      },
      {
        "targetIndex": 1,
        "blocks": [
          {
            "opcode": "event_whenflagclicked",
            "topLevel": true
          },
          {
            "opcode": "looks_nextcostume"
          }
        ]
      },
      {
        "targetIndex": 2,
        "blocks": [
        ]
      }
    ]
  }
 ```