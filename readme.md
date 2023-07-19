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
        "blocks": {
          "includeMatch": [
            [
              {
                "opcode": "event_whenkeypressed",
                "topLevel": true,
                "fields": { "KEY_OPTION": ["*", null] }
              },
              {
                "opcode": "sound_play",
                "inputs": { "SOUND_MENU": [1, "*"] }
              },
              {
                "opcode": "sound_sounds_menu",
                "fields": { "SOUND_MENU": ["*", null] }
              }
            ],
            [
              {
                "opcode": "event_whenflagclicked",
                "topLevel": true
              },
              {
                "opcode": "looks_say",
                "inputs": { "MESSAGE": [1, [10, "*"]] }
              }
            ]
          ],
          "exactMatch": [
            {
              "opcode": "looks_say"
            }
          ]
        }
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

## Dive
### Blocks
![Dive](/Dive.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Pool"
          },
          {
             "name": "Underwater 1"
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
            "opcode": "looks_changesizeby",
            "inputs": { "CHANGE": [1, [4, "*"]] }
          }
        ]
      },
      {
        "targetIndex": 2,
        "blocks":[],
        "name": "Diver2"
      }
    ]
  }
 ```



 ## Forest
### Blocks
![Forest](/Forest.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Castle 2"
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
          },
          {
            "opcode": "looks_think",
            "inputs": { "MESSAGE": [1, [10, "*"]] }
          },
          {
            "opcode": "event_whenkeypressed",
            "topLevel": true
          },
          {
            "opcode": "motion_movesteps",
            "inputs": { "STEPS": [1, [4, "*"]] }
          }
        ]
      },
      {
        "targetIndex": 2,
        "blocks": []
      }
    ]
  }
 ```




 ## Fox
### Blocks
![Fox](/Fox.jpg)
![Fox1](/Fox1.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Jungle"
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
            "opcode": "looks_changesizeby",
            "inputs": { "CHANGE": [1, [4, "*"]] }
          }
        ]
      },
      {
        "targetIndex": 2,
        "blocks": [
          {
            "opcode": "event_whenflagclicked",
            "topLevel": true
          },
          {
            "opcode": "motion_gotoxy",
            "inputs": { "X": [1, [4, "*"]], "Y": [1, [4, "*"]] }
          }
        ]
      }
    ]
  }
 ```


 ## Frog
### Blocks
![Frog](/Frog.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Pathway"
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
            "opcode": "looks_switchcostumeto",
            "inputs": { "COSTUME": [1, "*"] }
          },
          {
            "opcode": "looks_costume"
          }
        ]
      },
      {
        "targetIndex": 2,
        "blocks":[],
        "name": "Diver2"
      }
    ]
  }
 ```




  ## Graph
### Blocks
![Graph](/Graph.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Xy-grid-20px"
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
                "opcode": "sound_play",
                "inputs": { "SOUND_MENU": [1, "*"] }
            },
            {
                "opcode": "sound_sounds_menu",
                "fields": { "SOUND_MENU": ["*", null] }
            },
            {
                "opcode": "looks_say",
                "inputs": { "MESSAGE": [1, [10, "*"]] }
            },
            {
                "opcode": "event_whenkeypressed",
                "topLevel": true,
                "fields": { "KEY_OPTION": ["*", null] }
            },
            {
                "opcode": "looks_think",
                "inputs": { "MESSAGE": [1, [10, "*"]] }
            },
            {
                "opcode": "motion_turnright",
                "inputs": { "DEGREES": [1, [4, "*"]] }
            },
            {
                "opcode": "event_whenthisspriteclicked",
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



  ## Hen
### Blocks
![Hen](/Hen.jpg)
![Hen1](/Hen1.jpg)
![Hen2](/Hen2.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Forest"
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
            "opcode": "looks_say",
            "inputs": { "MESSAGE": [1, [10, "*"]] }
          }
        ]
      },
      {
        "targetIndex": 2,
        "blocks": []
      },
      {
        "targetIndex": 3,
        "blocks": [
            {
              "opcode": "event_whenflagclicked",
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
      },
      {
        "targetIndex": 4,
        "blocks": [
            {
              "opcode": "event_whenflagclicked",
              "topLevel": true
            },
            {
              "opcode": "motion_movesteps",
              "inputs": { "STEPS": [1, [4, "*"]] }
            }
        ]
      }
    ]
  }
 ```


  ## Jungle
### Blocks
![Jungle](/Jungle.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Jungle"
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
            "opcode": "looks_say",
            "inputs": { "MESSAGE": [1, [10, "*"]] }
          }
        ]
      },
      {
        "targetIndex": 2,
        "blocks":[]
      }
    ]
  }
 ```


   ## Laptop
### Blocks
![Laptop](/Laptop.jpg)
![Laptop1](/Laptop1.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Bedroom 3"
          }
        ]
      },
      {
        "targetIndex": 1,
        "blocks": [
          {
            "opcode": "event_whenthisspriteclicked",
            "topLevel": true
          },
          {
             "opcode": "motion_gotoxy",
             "inputs": { "X": [1, [4, "*"]], "Y": [1, [4, "*"]] }
          },
          {
            "opcode": "motion_movesteps",
            "inputs": { "STEPS": [1, [4, "*"]] }
          }
        ]
      },
      {
        "targetIndex": 2,
        "blocks": [
          {
            "opcode": "event_whenflagclicked",
            "topLevel": true
          },
          {
             "opcode": "motion_movesteps",
             "inputs": { "STEPS": [1, [4, "*"]] }
          },
          {
            "opcode": "motion_movesteps",
            "inputs": { "STEPS": [1, [4, "*"]] }
          }
        ]
      }
    ]
  }
 ```



  ## Meraki
### Blocks
![Meraki](/Meraki.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0
      },
      {
        "targetIndex": 1,
        "blocks": [
          {
            "opcode": "event_whenflagclicked",
            "topLevel": true
          },
          {
            "opcode": "control_repeat",
            "inputs": {
              "TIMES": [1, [6, "*"]],
              "SUBSTACK": [2, "*"]
            }
          },
          {
            "opcode": "looks_say",
            "inputs": { "MESSAGE": [1, [10, "*"]] }
          },
          {
            "opcode": "motion_movesteps",
            "inputs": { "STEPS": [1, [4, "*"]] }
          }
        ]
      }
    ]
  }
 ```


  ## Merakii
### Blocks
![Merakii](/Merakii.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0
      },
      {
        "targetIndex": 1,
        "blocks": [
          {
            "opcode": "event_whenflagclicked",
            "topLevel":true
          },
          {
            "opcode": "motion_turnright",
            "inputs": { "DEGREES": [1, [4, "*"]] }
          },
          {
            "opcode": "event_whenkeypressed",
            "topLevel":true
          },
          {
            "opcode": "motion_turnleft",
            "inputs": { "DEGREES": [1, [4, "*"]] }
          }
        ]
      }
    ]
  }
 ```




  ## Neon
### Blocks
![Neon](/Neon.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Neon Tunnel"
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
            "opcode": "looks_changesizeby",
            "inputs": { "CHANGE": [1, [4, "*"]] }
          }
        ]
      }
    ]
  }
 ```


  ## Park
### Blocks
![Park](/Park.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Woods And Bench"
          }
        ]
      },
      {
        "targetIndex": 1,
        "blocks": [
          {
            "opcode": "event_whenthisspriteclicked",
            "topLevel": true
          },
          {
            "opcode": "looks_say",
            "inputs": { "MESSAGE": [1, [10, "*"]] }
          },
          {
            "opcode": "looks_nextcostume"
          }
        ]
      },
      {
         "targetIndex": 2,
         "blocks":[],
         "name": "Owl"
      }
    ]
  }
 ```



 ## Planet
### Blocks
![Planet](/Planet.jpg)
![Planet1](/Planet1.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Stars"
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
            "opcode": "motion_turnright",
            "inputs": { "DEGREES": [1, [4, "*"]] }
          }
        ]
      },
      {
        "targetIndex": 2,
        "blocks": [
            {
              "opcode": "event_whenkeypressed",
              "topLevel": true
            },
            {
              "opcode": "motion_movesteps",
              "inputs": { "STEPS": [1, [4, "*"]] }
            }
        ]
      }
    ]
  }
 ```


  ## Princess
### Blocks
![Princess](/Princess.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "Theater"
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
            "opcode": "looks_say",
            "inputs": { "MESSAGE": [1, [10, "*"]] }
          }
        ]
      }
    ]
  }
 ```


 ## School
### Blocks
![School](/School.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes": [
          {
            "name": "School"
          },
          {
            "name": "Night City With Street"
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
            "opcode": "looks_switchbackdropto",
            "inputs": { "BACKDROP": [1, "*"] }
          },
          {
            "opcode": "looks_backdrops"
          }
        ]
      }
    ]
  }
 ```


 ## Steps
### Blocks
![Steps](/Steps.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0
      },
      {
        "targetIndex": 1,
        "blocks": [
          {
            "opcode": "event_whenflagclicked",
            "topLevel":true
          },
          {
            "opcode": "motion_movesteps",
            "inputs": { "STEPS": [1, [4, "*"]] }
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



 ## Teacher
### Blocks
![Teacher](/Teacher.jpg)
![Teacher1](/Teacher1.jpg)

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
            "opcode": "looks_say",
            "inputs": { "MESSAGE": [1, [10, "*"]] }
          }
        ]
      },
      {
        "targetIndex": 2,
        "blocks": [
          {
            "opcode": "event_whenflagclicked",
            "topLevel": true
          },
          {
            "opcode": "motion_turnright",
            "inputs": { "DEGREES": [1, [4, "*"]] }
          }
        ]
      }
    ]
  }
 ```



  ## Truck
### Blocks
![Truck](/Truck.jpg)

### Solution

``` javascript 
"solution": {
    "targets": [
      {
        "targetIndex": 0,
        "costumes":[
            {
                "name":"Street"
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
      }
    ]
  }
 ```