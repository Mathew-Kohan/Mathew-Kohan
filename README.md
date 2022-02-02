### Hi there, I’m @Mathew-Kohan 👋


- 👀 I’m interested in games development.
- 🌱 I’m currently learning C# and Unity.
- 💞️ I’m looking to collaborate on Game jams.
- ⚡ Fun fact: Game Jams are delicious.
- 😄 Pronouns: ... He/Him
- 📫 How to reach me =>
[Twitter](https://twitter.com/mh_kl)
[Discord](https://discord.com/users/855715968533135370)
[Instagram](https://www.instagram.com/mh.kay/)


function startGame() {
  myGamePiece = new component(30, 30, "red", 10, 120);
  myGamePiece.gravity = 0.05;
  myScore = new component("30px", "Consolas", "black", 280, 40, "text");
  myGameArea.start();
}

var myGameArea = {
  canvas : document.createElement("canvas"),
  start : function() {
    this.canvas.width = 480;
    this.canvas.height = 270;
    this.context = this.canvas.getContext("2d");
    document.body.insertBefore(this.canvas, document.body.childNodes[0]);
    this.frameNo = 0;
  },
  clear : function() {
    this.context.clearRect(0, 0, this.canvas.width, this.canvas.height);
  }
}

