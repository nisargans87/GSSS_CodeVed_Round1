# Technical Snake Game – CodeVed Round 1

> An interactive Snake Game combining technical MCQ challenges with time-based gameplay.

## Project Overview

Technical Snake Game is a browser-based game built for **Round 1** of **CodeVed**, a technical event conducted during **Gita Samhita – 2025** at **GSSS SSFGC, Mysuru**. It combines traditional Snake gameplay with technical multiple-choice questions: collecting an apple brings up a question, and a correct answer earns a point and grows the snake.

## About the Event

**Gita Samhita – 2025** is the annual college festival at **GSSS SSFGC, Mysuru**. **CodeVed** was conducted as a technical event as part of the festival. This Technical Snake Game was developed for Round 1 of the event.

## Key Features

- Classic Snake gameplay rendered on an HTML5 canvas
- Arrow-key controls with checks against immediately reversing direction
- Technical MCQs on programming, databases, operating systems, networking, AI, OOP, and related concepts
- Random question selection without repeats until the question pool has been used; the pool then resets
- Score tracking and snake growth after a correct answer
- A 15-minute countdown with a visual time-progress bar
- Random apple placement
- Boundary and self-collision detection
- Game-over handling for collisions and timer expiry
- Snake movement pauses while the MCQ is displayed; the countdown continues

## How the Game Works

1. The game starts with a snake, an apple, and a 15-minute countdown.
2. Use the arrow keys to steer the snake toward the apple.
3. When the snake collects an apple, a technical MCQ appears and snake movement pauses.
4. Submit an answer to continue. A correct answer increases the score and grows the snake; an incorrect answer does not increase the score or grow the snake.
5. The submitted question is removed from the current pool. Once all questions have been used, the pool is replenished.
6. A new apple is generated after the answer is submitted.
7. The game ends if the snake hits a boundary or itself, or when the countdown expires. The final score is shown in an alert.

## Technology Stack

| Technology | Purpose |
| --- | --- |
| HTML5 | Page structure and MCQ interface |
| CSS3 | Styling, layout, game interface, and visual effects |
| JavaScript | Game logic, controls, questions, scoring, and timer |
| HTML5 Canvas | Rendering the snake, apple, and game area |
| DOM API | Updating the score, timer, questions, options, and interface |
| Keyboard events | Reading arrow-key controls |
| JavaScript timers | Running the game loop and countdown |

## Project Structure

```text
.
├── README.md
└── Snake_Game.html
```

## Installation and Setup

Clone the repository and move into its directory:

```bash
git clone <repository-url>
cd <repository-folder>
```

Open `Snake_Game.html` directly in a modern web browser to play. For local development, you can optionally open the project in VS Code and use the Live Server extension.

## How to Play

- Use the arrow keys to control the snake.
- Collect apples to bring up technical MCQs.
- Answer each question to resume snake movement.
- Correct answers increase the score and snake length.
- Avoid the game boundaries and the snake itself.
- Complete the challenge before the 15-minute timer expires.

## Technical Implementation

- **Canvas rendering:** Draws the game area, snake, and apple.
- **Game loop:** `setInterval()` calls the drawing and movement function every 300 milliseconds.
- **Snake state and movement:** An array of grid coordinates represents the snake; keyboard event listeners update its direction.
- **Collision detection:** Checks the next head position against the canvas boundaries and existing snake segments.
- **Food positioning:** Generates apple coordinates on the game's grid using random values.
- **Question management:** Stores questions and options as objects in an array, selects randomly from the available pool, removes a question after submission, and restores the pool after it is exhausted.
- **Question interface:** Updates the question and answer options through DOM manipulation and radio inputs.
- **Scoring and growth:** Updates the displayed score and adds a snake segment after a correct response.
- **Pause and resume:** Stops snake drawing and movement while the question is open, then resumes after an answer is submitted.
- **Countdown and progress:** Uses a one-second timer to update the displayed time and the width of the visual progress bar. The countdown continues while a question is open.

## Learning Outcomes

This project demonstrates practical use of:

- JavaScript fundamentals, arrays, objects, and conditional logic
- DOM manipulation and keyboard event handling
- The HTML5 Canvas API and game-loop logic
- Randomization and collision detection
- Score and timer updates in an interactive interface
- UI design and problem-solving
- Integrating educational content into an interactive web application

## Future Enhancements

The following are possible future improvements and are not currently implemented:

- Difficulty levels and multiple game modes
- Sound effects and improved animations
- High-score storage and persistent player scores
- Responsive or mobile controls
- Additional technical question categories
- A leaderboard
- Backend-based question management

## Screenshots / Demo

Screenshots can be added to this section to demonstrate the game interface, MCQ popup, scoring system, and timer.

## Project Highlights

**Gaming + Technical Knowledge + Time-Based Challenge**

The project pairs familiar Snake gameplay with technical questions triggered by collected apples. A countdown adds a time limit to the challenge, while correct answers reward the player with points and a longer snake.

## Event Information

| Detail | Information |
| --- | --- |
| Event | CodeVed |
| Festival | Gita Samhita – 2025 |
| Institution | GSSS SSFGC, Mysuru |
| Category | Technical Event |
| Round | Round 1 |
| Project | Technical Snake Game |

## Author / Developer

**Developed by**

`Your Name`

- GitHub: [Profile link]
- LinkedIn: [Profile link]
- Email: [Email address]