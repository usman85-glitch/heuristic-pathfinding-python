# Heuristic Pathfinding with Backtracking

A Python-based navigation engine developed to explore graph theory and search optimizations. This script implements a hybrid approach, using A* metrics to prioritize movement while maintaining a custom stack to handle complex backtracking scenarios.

### Technical Highlights
- **Heuristic Evaluation:** Calculates total cost ($f = g + h$) to ensure the most promising nodes are explored first.
- **Stack-Based Backtracking:** Uses a manual state-recovery system to revert from dead ends and explore alternative routes without getting stuck in local optima.
- **Cycle Prevention:** Implements dynamic path-checking to prevent infinite loops in cyclic graphs.
- **Data Parsing:** Dynamically builds node and edge objects from a custom schema in `map.txt`.

### File Structure
- `pathfinding.py`: The core algorithm logic.
- `map.txt`: The input data file containing node heuristics and adjacency lists.

### How to Run
1. Ensure `map.txt` is in the same directory as the script.
2. Run `python pathfinding.py`.
3. Input the start and end nodes when prompted (e.g., `A1` and `A10`).
