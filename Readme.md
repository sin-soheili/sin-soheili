# About Me

## Personal Information
- Name: [Setayesh]
- Age: <span style="color: blue;">18 years old</span>
- Email: [sin.soheili@hotmail.com](mailto:sin.soheili@hotmail.com)

## Skills
- Programming Languages: <span style="color: green;">Python (Junior level)</span> , <span style="color: yellow;">JavaScript</span>
- Web Technologies: HTML, CSS, JavaScript, Tailwind, Sass, Bootstrap

## Education and Experience
- Currently studying software engineering
- Exploring FastAPI for enhancing web development skills

## Interests and Passions
- Passionate about Python and scripting
- Interested in web development and working with various frameworks and libraries

## Contact Me
- Email: [sin.soheili@hotmail.com](mailto:sin.soheili@hotmail.com)
- GitHub: [https://github.com/sin-soheili]

## Tic-Tac-Toe Game

Try playing Tic-Tac-Toe with me!

<!DOCTYPE html>
<html>
<head>
  <title>Tic-Tac-Toe</title>
  <style>
    .board {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      grid-template-rows: repeat(3, 1fr);
      gap: 5px;
    }

    .cell {
      border: 1px solid black;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 48px;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <h1>Tic-Tac-Toe</h1>
  <div class="board">
    <div class="cell"></div>
    <div class="cell"></div>
    <div class="cell"></div>
    <div class="cell"></div>
    <div class="cell"></div>
    <div class="cell"></div>
    <div class="cell"></div>
    <div class="cell"></div>
    <div class="cell"></div>
  </div>

  <script>
    const cells = document.querySelectorAll('.cell');
    let currentPlayer = 'X';

    cells.forEach(cell => {
      cell.addEventListener('click', handleCellClick);
    });

    function handleCellClick(event) {
      const selectedCell = event.target;
      if (selectedCell.textContent === '') {
        selectedCell.textContent = currentPlayer;
        currentPlayer = currentPlayer === 'X' ? 'O' : 'X';
      }
    }
  </script>
</body>
</html>
