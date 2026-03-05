# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A single-file Tic Tac Toe game (`index.html`) with no build system, dependencies, or package manager. Open the file directly in a browser to run it.

## Architecture

Everything lives in `index.html` — HTML structure, CSS styles, and JavaScript logic are all inline in one file.

**Key JS concepts:**
- `board` — 1D array of 9 strings (`''`, `'X'`, or `'O'`) representing the grid
- `WINS` — hardcoded array of all 8 winning index combinations
- `checkWinner()` — iterates `WINS`, returns `'X'`, `'O'`, `'D'` (draw), or `null`
- Score state (`score.X`, `score.O`, `score.D`) persists across games via `init()` resets only the board, not the score

## Git Workflow

**Every change must be committed and pushed to GitHub — no exceptions.**

- After completing any task or modification, stage the relevant files, create a commit, and push to `main`
- Commit messages must be clear and descriptive: summarize *what* changed and *why* in the subject line (imperative mood, e.g. "Add win highlight animation" not "added stuff")
- Never leave uncommitted changes at the end of a session
- This ensures all work is preserved and any change can be reverted if needed

**Repo:** https://github.com/igorstoyanov/ai-test — branch `main`
