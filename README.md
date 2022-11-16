<h1 align="center">
  <img src="images/stein_gate.png">
</h1>

# My Game - Steins;Gate

Course: CIS 700 Interactive Fiction and Text Generation. Advisors Prof. Chris Callison-Burch and Dr. Lara Martin.

* [notebook](my_game_with_pixray.ipynb)
* [roadmap](my_game_visual.pdf)
* [playthrough](playthrough.txt) ([detailed version](playthrough_with_description.txt)) 

##  Game Description

This game named [*Steins;Gate*](https://store.steampowered.com/app/412830/STEINSGATE/), derived from [the famous anime with the same name](https://en.wikipedia.org/wiki/Steins;Gate_(TV_series)). It begins with a rag-tag band of tech-savvy young students who discover the methods of changing the past via mail, using a modified microwave. Later, you (Rintaro) and your teammates are involved into a seires of tasks and consequences, including 

1.   The death of Kurisu, your lover and the time machine theory founder
2.   The coming World War III triggered by the invention of time machine

In our game, we focus on the last part of the story. That is, you should travel back to a month ago to 

1.   Save your lover (Kurisu) by deceiving the world

2.   Destroy the time machine paper taken by Kurisu's father to avoid Word War III

Your different action will lead to different timeline! There're **4 timelines** waiting for you to explore!

## About Pixray 

The game can generate [the images of location and item](./images) by the selected art style from [pixray](https://github.com/pixray/pixray). 

We  generate the images of location and item by given different art styles (`drawer`) and prompt. Specifically, as for the prompt engineering, we follow the [official instruction](https://dazhizhong.gitbook.io/pixray-docs/docs/primary-settings) and weight the objects by importance during simultaneous prompting. We also try to avoid unwanted objects by setting negative weight with early stop. Both techniques work. Finally, we use two art styles, namely `pixel` and `clipdraw`, to render the images successfully. 

For more detail, see  [this notebook](pixray_location_item.ipynb).

## Demo

In this game, the location and stationary items will pop out once you arrive at that location. The accessible items will show when you check your inventory in the game.

### Demo 1 - Anime Style

<h1 align="center">
  <img src="demo/demo_anime.jpg" width="400">
</h1>

### Demo 2 - Clipdraw Style

<h1 align="center">
  <img src="demo/demo_clipdraw.jpg" width="400">
</h1>

### Demo 3 - Pixel Style

<h1 align="center">
  <img src="demo/demo_pixel.jpg" width="400">
</h1>

## Why to Choose This Topic

Time travel is a funny and timeless sci-fi topic, and it can trigger different endings (both happy ending and bad ending) by differenct implemetation. It's quite challenging yet interesting to adapt the in-class interactive text game into a new time travel game.
