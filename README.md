Simple Game of Cricket using HTML, CSS and JS

game.css

#body {
  position: relative;
  padding-top: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  color:blue;
}

#body::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-image: url('./pngtree-cricket-logo-png-image_8823326.png');
  background-size: cover;
  background-position: center;
  filter: blur(5px);
  z-index: -1;
}

.button {
  font-size: large;
  font-family: 'Times New Roman', Times, serif;
  margin-right: 10px;
  border: 2px solid black;
  background-color: aqua;
  color: darkred;
}

#button {
  font-size: larger;
}

.foot {
  margin-top: 50px;
  text-align: center;
  justify-content: center;
  color: yellow;
}


game.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cricket</title>
  <link rel="stylesheet" href="./game.css">
</head>
<body id="body">
  <div>
    <h1>Bat Ball Stump Game</h1>
  </div>
  <div>
    <button class="button" onclick="
      console.log('Bat Button Clicked');
      const rand = Math.random() * 3;
      let cchoice;
      if (rand > 0 && rand <= 1) {
        cchoice = 'Bat';
        console.log('Computer Choice is Bat');
      } else if (rand > 1 && rand <= 2) {
        cchoice = 'Ball';
        console.log('Computer Choice is Ball');
      } else {  
        cchoice = 'Stump';
        console.log('Computer Choice is Stump');
      }
      if (cchoice === 'Bat') {
        console.log('Computer Won');
      } else if (cchoice === 'Ball') {
        console.log('It\'s a Tie');
      } else {
        console.log('User Won');
      }
    ">Bat</button>
    <button class="button" onclick="
      console.log('Ball Button Clicked');
      rand = Math.random() * 3;
      if (rand > 0 && rand <= 1) {
        cchoice = 'Bat';
        console.log('Computer Choice is Bat');
      } else if (rand > 1 && rand <= 2) {
        cchoice = 'Ball';
        console.log('Computer Choice is Ball');
      } else {
        cchoice = 'Stump';
        console.log('Computer Choice is Stump');
      }
      if (cchoice === 'Bat') {
        console.log('Computer Won');
      } else if (cchoice === 'Ball') {
        console.log('It\'s a Tie');
      } else {
        console.log('User Won');
      }
    ">Ball</button>
    <button class="button" onclick="
      console.log('Stump Button Clicked');
      rand = Math.random() * 3;
      if (rand > 0 && rand <= 1) {
        cchoice = 'Bat';
        console.log('Computer Choice is Bat');
      } else if (rand > 1 && rand <= 2) {
        cchoice = 'Ball';
        console.log('Computer Choice is Ball');
      } else {
        cchoice = 'Stump';
        console.log('Computer Choice is Stump');
      }
      if (cchoice === 'Bat') {
        console.log('Computer Won');
      } else if (cchoice === 'Ball') {
        console.log('It\'s a Tie');
      } else {
        console.log('User Won');
      }
    ">Stump</button>
  </div>
  <div class="foot">
    <h1>Rules for the Game</h1>
    <h3>1. If You Clicked Bat & Computer Chose Bat Then Computer Won</h3>
    <h3>2. If You Clicked Bat & Computer Chose Stump Then You Won</h3>
    <h3>3. If You Clicked Bat & Computer Chose Ball Then It is a Tie</h3>
    <h3>4. If You Clicked Ball & Computer Chose Bat Then Computer Won</h3>
    <h3>5. If You Clicked Ball & Computer Chose Ball Then It is a Tie</h3>
    <h3>6. If You Clicked Ball & Computer Chose Stump Then You Won</h3>
    <h3>7. If You Clicked Stump & Computer Chose Bat Then Computer Won</h3>
    <h3>8. If You Clicked Stump & Computer Chose Ball Then It is a Tie</h3>
    <h3>9. If You Clicked Stump & Computer Chose Stump Then You Won</h3>

    <h1>See Results in Console</h1>

  </div>
</body>
</html>


