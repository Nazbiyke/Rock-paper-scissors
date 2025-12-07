# Rock–Paper–Scissors Game of Life #

## Project Description ##

This project is my attempt to create a simplified Rock–Paper–Scissors version of Conway’s Game of Life. I was inspired by a TikTok video showing groups of “rocks,” “scissors,” and “papers” moving randomly and transforming when they encountered each other. When two elements met:
- Scissors that touched rocks became rocks
- Papers touching scissors became scissors
- Rocks touching papers became papers
  
Based on that idea, I decided to build my own minimal implementation. For reference, I used an example code provided on OCS.

### **Rules of the Simulation** ###

Cell Types
- Rock = black
- Scissors = yellow
- Paper = pink

### **Interaction Rules**

The logic follows the classic Rock–Paper–Scissors cycle:
- Scissors beat Paper
- Paper beats Rock
- Rock beats Scissors

**Survival Rules**

 A cell survives under the following conditions:
1. It is stronger than its neighbor(s).
    - Example: scissors kill any paper neighbor and therefore survive.
2. It has no neighbors at all.
    - A cell without adjacent opponents remains alive.
Conversely, a cell dies if any neighboring cell beats it.
Example: if a scissors cell has at least one rock neighbor, it turns into a rock.

![tk 06 04 2022 19_51_11](https://user-images.githubusercontent.com/100347662/162035677-40c35767-61de-4540-af0f-30d1e5a58497.png)

