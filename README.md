# HtmlCanvasGame

## 2023/10/23: The idea

* Make a game with my son
* Teach him some basic coding

Brainstorming with him...

### Scoring

* Best score
* Current score (while playing the game you can see your score)
* End Of Game Score/Event

```
On End Of Game Event
  If higher Current Score than Best Score
    Change Best Score to Current Score
  End If

  Show End Of Game Screen
End
```

### Title Screen

* Displays Best Score
* Play Button

```
On Play Button Click
   Set Current Score to zero
   Show Game Screen
End
```

### End Of Game Screen

* Game Over Message
* Current Score
* Best Score
* Play Button (see Title Screen)

### Start

* Show Title Screen

### Game Screen

* ???? :)

## 2023/11/01: JavaScript Canvas API

After the idea chat, I thought I'd look into the HTML Canvas API, I've seen people play about with it for games over the years, but I've never looked at it, until today.

I started here: https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API

Looks pretty simple, so I made some ugly squares, I'll commit some code for it.