# audio-player
This is inspired by the series of "Build An Audio Player Using HTML5 &amp; jQuery" which is made by Traversy Media. As soon as I saw the video tutorials, it came to my mind that it would be a good idea if I get that idea and turn it into one using vanilla JavaScript. And I got around to get inspired on the UIs for the audio player. I found a kickass design which is made and owned by "Giga Tamarashvili"

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Audio Player using HTML5 Audio API</title>
  <link href="https://fonts.googleapis.com/css2?family=Nunito:wght@200;400;600;800&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="./css/reboot.css">
  <link rel="stylesheet" href="./css/styles.css">
</head>
<body>
  <div class="player-wrap d-flex flex-column">
    <header class="player-head d-flex">
        <button type="button" class="btn--prev d-flex" title="Back to the list">
          <img src="./img/rounded-left.svg" class="arrow" alt="#">
        </button>
        <strong>Song</strong>
        <button type="button" class="btn--menu d-flex" title="Watch the menu">
          <img src="./img/more-horizontal-outline.svg" class="dot3" alt="#">
        </button>
    </header>
    <main class="player-main d-flex flex-column">
      <div class="group--meta d-flex flex-column">
        <img alt="cover image" class="cover-image" src="./img/@temp-cover.png">
        <h1 class="song-title">Snowmine</h1>
        <strong class="song-artist">Let me in</strong>
      </div>
      <div class="group--progress d-flex">
        <span id="time-gone" class="time-marker time--gone">00:00</span>
        <div id="progressbar" class="progressbar">
          <span id="tracker" class="progressbar-tracker"></span>
        </div>
        <span id="time-left" class="time-marker time--left">03:50</span>
      </div>
      <div class="group--song-controller d-flex">
        <button class="btn--prev" type="button" id="prev" title="Go to the previous song">
          <img src="./img/arrow-left.svg" alt="#">
        </button>
        <button class="btn--play" type="button" id="play" title="Play the song">
          <img src="./img/play.svg" alt="#">
        </button>
        <button class="btn--pause" type="button" id="pause" title="Pause the song">
          <img src="./img/stop.svg" alt="#">
        </button>
        <button class="btn--next" type="button" id="next" title="Go to the next song">
          <img src="./img/arrow-right.svg" alt="#">
        </button>
      </div>
      <div class="group--play-controller d-flex">
        <button type="button" id="prev" title="shuffle" class="btn--shuffle">
          <img src="./img/shuffle-2-outline.svg" alt="#">
        </button>
        <button type="button" id="play" class="btn--lyrics">Lyrics</button>
        <button type="button" id="pause"title="repeat" class="btn--repeat">
          <img src="./img/repeat-outline.svg" alt="#">
        </button>
      </div>
    </main>
  </div>
</body>
</html>
