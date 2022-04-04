# ZWordle
([wordle](https://www.powerlanguage.co.uk/wordle/) for zsh - with tab completion!)

[![asciicast](https://asciinema.org/a/W8SzmrTF9k5JcoGnlUSOGfNOs.svg)](https://asciinema.org/a/W8SzmrTF9k5JcoGnlUSOGfNOs)

## Usage
### Playing
_This mode plays wordle's word of the day by default. Or any other day's word using eg. `num=1038`._
```
zwordle
```
<img width="345" alt="Screen Shot 2022-04-04 at 09 39 37" src="https://user-images.githubusercontent.com/49626717/161454154-3a22f585-4b01-476b-aff1-7386349d521c.png">



### Solving
_This mode helps you solve other wordles, but requires you to score your own words._

Examples:
 * `.` (for any ⬜ letter)
 * uppercase `W` (for a 🟩 `W`)
 * lowercase `i` (for a 🟨 `I`)

First initialize zwordle's zsh tab completion, this can be done with:
```
source zwordle
```

*Then* the following should work in zsh:
```
zwordle weary=W.... pills=.i<TAB>
```
<img width="355" alt="Screen Shot 2022-04-04 at 09 33 23" src="https://user-images.githubusercontent.com/49626717/161453711-9f098dc6-b5d4-48fb-9f40-536f121389e4.png">


```
zwordle weary=W.... pills=.i... vague=..... <TAB>
```
<img width="555" alt="Screen Shot 2022-04-04 at 09 00 53" src="https://user-images.githubusercontent.com/49626717/161452574-07d86f06-2c09-434d-89a6-3595bbef4fec.png">

### Solving (multi)
_([dordle](https://zaratustra.itch.io/dordle) or [quordle](https://www.quordle.com/) or ...)_
```
zwordle radio=Ra...=r...o=....o=R...o rumba=RU..a=rU...=..M..=R.... rural=RURAL=.UR..=....l=R.... furor==.UROR=...O.=..ro. juror==JUROR=...O.=..ro. lemon===LEMON=...o. rocks====ROCKS
```
<img width="1007" alt="Screen Shot 2022-04-04 at 10 44 55" src="https://user-images.githubusercontent.com/49626717/161456953-19b9cfc5-b391-4a59-8b27-3334eb835083.png">


## Installation
```
git clone https://github.com/zechris/zwordle.git ~/Code/zechris/zwordle
export PATH="$PATH:$HOME/Code/zechris/zwordle/bin"
```

### Why?
Because I wanted to learn more about zsh & tab completion.

Oh, and to cheat at https://www.quordle.com ... that game does my head in!
