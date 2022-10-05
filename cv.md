# Weronika Dziura

## Contact details

**Phone:** +00 000 000 000

**E-mail:** wer.dziura@gmail.com

**LinkedIN:** https://www.linkedin.com/in/weronika-dziura/

**GitHub:** https://github.com/werdziur

**Location:** Cracow, Poland
## About me

I am a reliable and committed professional with 5 years of practical experience in finance area. 
I am characterized by a high work ethic and analytical approach to the assigned tasks. I feel natural in being accountable for the delegated tasks, and roles. 
One of my strongest competencies is pursuing for self-development. 

**I have started learning programming at the beggining of 2022 and it has become my main goal and desire for the future. I feel great while coding, it makes me happy and fullfill. Currently, I am taking part in Frontend course in RSSchool as well as JavaScript course on Teachable** 
I am willing to use the opportunities given by the company to develop my skills and improve my daily work, then. I successfully establish contacts with other people, both on business and private level. 
After hours, I am interested in fitness, dietetics, crocheting and reading books.

## Education

**2022** - RSSchool - FrontEnd course

**2022** - HTML, CSS, Responsive Web Design and JavaScript course on Udemy/Teachable/LinkedIn.

**2020** - *Discover IT Program* aiming to get OPS workers familiar with the software development principles, Agile approach, Scrum framework, and testing.

**2019** - HTML, CSS 2-days stationary course

**2016** - 2018 Jagiellonian University, Cracow, Faculty of Economics - Corporate Finance & Accounting (Master’s Degree).

**2013** - 2016 Jagiellonian University, Cracow, Faculty of Economics - Finance, Banking, Insurances (Bachelor’s degree).



## Skills

- Knowledge of MS Office Suite
- Precision, ability to work in a team, organization skills, adaptability, high work ethic, willingness to learn
- Working under pressure and time management
- Strong attention to details
- Effective duties prioritization
- Agile working approach

## Stack

- HTML, CSS
- JavaScript - Basic
- qTest, Jira, Confluence – Foundations
- Visual Studio Code
- Git and GitHub

### Code example:

A part of a code to create a ScoreKeeper. At the beginning players have a possibility to add their names (but it is not necessary). Playing treshold from 6 points to max 10. Players can choose the convinient number. After achiving max points by winner, players can either reset the game of start new game. Winnings are authomatically counted in the table under the winner name after clicking RESET. NEW GAME button resume the game and remove wins from the table.

```
// Scorekeeper logic

let btnReset = document.querySelector('#btnreset');
const select = document.querySelector('#select');
let winningScore = 6;
let isGameOver = false;

let playerOneWins = document.querySelector('#playeronewins');
let playerTwoWins = document.querySelector('#playertwowins');
const btnRenew = document.querySelector('#renewgame');

let p1 = {
    button: document.querySelector('#btnone'),
    display: document.querySelector('#one'),
    score: 0,
    name: inputOne,
    winner: 0,
}

let p2 = {
    button: document.querySelector('#btntwo'),
    display: document.querySelector('#two'),
    score: 0,
    name: inputTwo,
    winner: 0,
}

function updateScores(competitorOne, competitorTwo) {
    if (!isGameOver) {
        competitorOne.score++;

    } if (competitorOne.score === winningScore) {
        isGameOver = true;
        competitorOne.display.classList.add('winner');
        competitorTwo.display.classList.add('loser');
        competitorOne.button.disabled = true;
        competitorTwo.button.disabled = true;
        competitorOne.winner++
        playerOneWins.textContent =
            `${competitorOne.name.toUpperCase()}: ${competitorOne.winner}`;
        playerTwoWins.textContent =
            `${competitorTwo.name.toUpperCase()}: ${competitorTwo.winner}`;
    }

    competitorOne.display.innerText = competitorOne.score;
}

p1.button.addEventListener('click', function () {
    updateScores(p1, p2)
});

p2.button.addEventListener('click', function () {
    updateScores(p2, p1)
});

btnReset.addEventListener('click', reset);

function reset() {
    isGameOver = false;
    p1.display.innerText = '0';
    p2.display.innerText = '0';
    p1.score = 0;
    p2.score = 0;
    p1.display.classList.remove('winner', 'loser');
    p2.display.classList.remove('winner', 'loser');
    p1.button.disabled = false;
    p2.button.disabled = false;
};

select.addEventListener('change', function () {
    reset();
    winningScore = parseInt(this.value);
    playerOneWins.textContent = 'Player One';
    playerTwoWins.textContent = 'Player Two';
    p1.winner = 0;
    p2.winner = 0;
})


btnRenew.addEventListener('click', function () {
    reset();
    playerOneWins.textContent = 'Player One';
    playerTwoWins.textContent = 'Player Two'
    p1.winner = 0;
    p2.winner = 0;
})

```


## Languagues

- English, C1, both spoken and written. I actively use English on daily basis in my current work
- German - A1 - learning in progress. I am taking part in a german course in my current workplace
- Polish - native

## Interest

- Programming :)
- Volunteering for animals (Shelter - Krakow
  Society for the Care of Animals)
- Nutrition in sports and strength sports
- Healthy lifestyle
- Popular science programs
- Crime stories and movies