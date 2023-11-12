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

Looks pretty simple, so I made some ugly squares, I'll commit some code for it: [20231101-ugly-squares.html](20231101-ugly-squares.html)

## 2023/11/11: Draw three squares

Squares A, B and C.

We want the squares to move slowly around.

To achieve this we need to render a frame, wait some time then re-render, and keep doing this. Between each render we want to adjust the location of each square.

We need a render function:

```
render()
  move A => xA = xA + 1; yA = yA + 1;
  (same for B and C)
  draw A
  draw B
  draw C
end
```
Call render every 25 milliseconds so we have (1000/25 = 40) ~40 FPS.

Not sure exactly how much to move by, but will try something out.

Here's how it went: [20231111-three-squares-that-move.html](20231111-three-squares-that-move.html)

Some additional tinkering on my own to add a crude FPS counter: [20231111-three-squares-that-move-plus-fps.html](20231111-three-squares-that-move-plus-fps.html)