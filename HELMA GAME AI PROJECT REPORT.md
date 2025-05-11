**Project Title:** *Helma: A Strategic Multiplayer Grid Capture Game*  
**Submitted By:**

* Yousuf Jamal (22K-5051) – *Team Leader*

* Abdul Mateen (22K-5070) – *Member*

* M. Mufrah Jawaid (22K-5046) – *Member*  
  **Course:** AI  
  **Instructor:** \[Alishba Subhani\]  
  **Submission Date:** \[11th-MAY-2025\]

**1\. Executive Summary**

**Project Overview:**  
This project involves the development of *Helma*, a custom-designed, turn-based strategic board game for three players. The game is played on a 8x8 grid and incorporates unique elements such as power tiles and rotating board sections to increase complexity. The project’s core objective was to design an AI capable of playing Helma strategically using the **Minimax algorithm with Alpha-Beta pruning** to make optimal moves in a competitive multiplayer environment.

---

**2\. Introduction**

**Background:**  
Traditional board games like chess and Ludo offer solid frameworks for strategic gameplay but typically cater to two players or lack dynamic changes in state. *Helma* is an original game conceptualized to challenge both human players and AI through strategic territory control, rotation mechanics, and pattern-based scoring. The game was selected for its potential to support innovative gameplay and AI experimentation.

**Objectives of the Project:**

* To design and implement a new board game with unique mechanics.

* To develop an AI agent capable of decision-making in a three-player environment.

* To utilize the Minimax algorithm (modified for multiplayer) along with Alpha-Beta pruning.

* To evaluate the AI’s performance against human and AI opponents.

**3\. Game Description**

**Original Game Rules:**  
As Helma is an original game, it has no direct predecessor. It takes inspiration from games like *Go*, *Blokus*, and *Othello*, focusing on territory control, pattern recognition, and positional strategy.

**Innovations and Modifications:**

* A 8x8 grid board with **power tiles** providing bonus effects.

* **15 tokens per player**, placed one at a time per turn.

* **Rotating board mechanics**: outermost row/column rotates after every three rounds.

* **Pattern-based scoring**: forming lines, corners, and special shapes earns points.

* **Power tiles** may allow an extra move, block, or special action.  
  These changes increase complexity, promote foresight, and ensure high replay value.

**4\. AI Approach and Methodology**

**AI Techniques Used:**

* **Minimax Algorithm**: Adapted for a three-player setting using a Max-N decision model.

* **Alpha-Beta Pruning**: Optimized the search tree by cutting off suboptimal branches.

* **(Optional)** Reinforcement Learning considered for future self-play enhancements.

**Algorithm and Heuristic Design:**

* Heuristic Function includes:

  * Points from patterns formed.

  * Control of power tiles.

  * Token positioning relative to opponents.

  * Defensive blocking potential.

  * Remaining token count advantage.

**AI Performance Evaluation:**

* Evaluated by simulating matches against human players.

* Measured **win rate**, **average decision time**, and **accuracy** of moves.

* Performance improved as heuristics were refined and alpha-beta pruning added.

**5\. Game Mechanics and Rules**

**Modified Game Rules:**

* Each player has 15 tokens.

* Board is 8x8 with special power tiles.

* Every 3 rounds, the outermost row or column rotates clockwise.

* Tokens are placed to form predefined scoring patterns (lines, corners, diagonals).

* Special tile actions can include:

  * Extra turn

  * Move opponent’s token

  * Protect a cell from future overwrite

**Turn-based Mechanics:**

* Player A → Player B → Player C (clockwise).

* Each player places one token per turn.

* After three complete rounds, the board changes dynamically.

**Winning Conditions:**

* Game ends when all players run out of tokens.

* Player with the highest score wins.

* Tie-breaker: fewest total moves used to gain score.

**6\. Implementation and Development**

**Development Process:**

* Game logic and AI core were developed in Python.

* GUI designed using Pygame.

* Game board and mechanics were built first, followed by integration of AI.

* AI tested iteratively with increasing search depths.

**Programming Languages and Tools:**

* **Programming Language:** Python

* **Libraries Used:**

  * Pygame – for GUI

  * NumPy – for matrix operations and board state management

* **Tools:**

  * GitHub – for version control

  * VS Code – main IDE used for development

**Challenges Encountered:**

* Implementing Minimax for 3 players required restructuring standard logic.

* Designing fair and efficient heuristics for a dynamic board state was complex.

* Maintaining UI responsiveness while AI computed moves was addressed using threading.

**7\. Team Contributions**

* **Yousuf Jamal (22K-5051):**

  * Team Lead

  * Designed and implemented the game interface using Pygame

  * Integrated AI logic with GUI

  * Oversaw project timeline and presentation

* **Abdul Mateen (22K-5070):**

  * Designed and implemented board mechanics and special rules

  * Handled board rotation logic and power tile effects

  * Documented rule sets and scoring logic

  * Developed the AI logic including  Alpha-Beta Pruning

* **M. Mufrah Jawaid (22K-5046):**

  * Developed the AI logic including Minimax 

  * Designed heuristic evaluation functions

  * Conducted performance testing and comparative analysis

**8\. Results and Discussion**

**AI Performance:**

* AI achieved a **win rate of 70%** against casual human players.

* With pruning enabled, average **decision time reduced to 1.8 seconds** per move.

* The heuristic allowed strategic placement and effective blocking.

* AI struggled slightly in end-game scenarios where dynamic rotations created unpredictable results — future improvements may include adaptive learning.

**9\. References**

* Russell, S., & Norvig, P. (2020). *Artificial Intelligence: A Modern Approach* (4th ed.). Pearson.

* GeeksforGeeks – [Minimax and Alpha-Beta Pruning tutorials](https://www.geeksforgeeks.org)

* Pygame Documentation – https://www.pygame.org/docs/

* Stack Overflow – For discussions on game rotation logic and event handling in Pygame

* Research papers on multi-agent Minimax and Max-N algorithms

