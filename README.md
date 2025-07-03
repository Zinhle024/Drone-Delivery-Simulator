📝 Project Overview – Delivery Drone Simulator

Welcome to the Delivery Drone Simulator project.

This is a beginner-friendly but realistic Java-based simulation where you’ll build and test a simple drone delivery system on a 2D grid. The project is designed to help you apply Java fundamentals (OOP, encapsulation, classes, methods), learn team-based GitHub collaboration, write tests using JUnit, and work within a structured development workflow.
🔍 Problem Description

Your task is to simulate a delivery drone system. The drone operates in a virtual 2D grid and can:

    Move in four directions (N, S, E, W),

    Avoid obstacles (like buildings or no-fly zones),

    Recharge its battery at charging stations, and

    Execute simple delivery commands.

You will write the logic that powers this drone, control its behavior via a set of instructions, and ensure everything is tested and modular.
🎯 Project Objectives

This project will help you:

    Practice Java fundamentals — classes, objects, methods, encapsulation, and inheritance.

    Learn clean architecture — organize code logically in packages (drone, world, commands, server).

    Collaborate with a team — using Git, GitHub branches, issues, and pull requests.

    Write and run tests — using JUnit to validate logic.

    Build confidence — writing code that doesn’t break, reading others’ code, and reviewing pull requests.

📦 Core Features You Must Implement
Feature	Description
2D Grid World	The drone moves on a grid with X, Y coordinates.
Drone Class	Stores name, position, direction, battery level.
Movement Commands	e.g., MOVE, TURN, REPORT.
Battery Logic	Drone consumes battery with every move and must recharge at stations.
Obstacles	Static obstacles the drone must detect and avoid.
Charging Stations	Allow the drone to restore full battery.
Command Parser	Receives and interprets user instructions.
Testing with JUnit	Each unit of logic must be tested and pass.
📁 Suggested Package Structure

src/
├── main/
│   └── java/com/deliverydrone/
│       ├── drone/         # Drone behavior
│       ├── world/         # Grid logic, obstacles, charging stations
│       ├── commands/      # Command pattern logic
│       └── Main.java      # Entry point
├── test/
│   └── java/com/deliverydrone/  # All JUnit test files

🧪 JUnit Testing Requirements

Every main class (Drone, Grid, ObstacleManager, CommandParser) should have test coverage. Test for:

    Moving with battery

    Moving into/around obstacles

    Charging logic

    Invalid commands

🚀 Stretch Goals (Optional)

If you finish early and want a challenge:

    Add random obstacle generation

    Support multiple drones

    Simulate real-time server-client behavior

    Add simple CLI or GUI interface

📌 Expectations

You’re expected to:

    Push to your own feature branch only

    Submit a pull request for every completed feature

    Review at least one teammate’s PR

    Write unit tests for the logic you implement

    Commit your code often with meaningful messages

💡 Reminder

    “If it’s not tested, it doesn’t work.”

This project is meant to make you comfortable with breaking problems down, working in teams, and writing Java confidently. Everything you need is either already assigned or documented. Before asking questions, check:

    The README

    Your Notion task board

    Existing code and examples
# Delivery Drone Simulator 🚁

A Java-based simulation of delivery drones navigating a grid world with obstacles, commands, and battery logic.

## 🌟 Overview

This project helps us practice Java fundamentals, JUnit testing, GitHub collaboration, and project planning.

## 👥 Team

| Name     | Role                | Skills                            |
|----------|---------------------|------------------------------------|
| Zinhle   | PM & Drone Logic    | Git, Learning Java                 |
| Lindiwe  | Command & Testing   | Java, Hardware                     |
| Dima     | Grid & Obstacles    | Java, Logic Structures             |

## ⚙️ Features

- 2D Grid World
- Drone movement & direction control
- Obstacles and charging stations
- Command Parser
- Battery logic
- JUnit Testing Suite

## 🛠️ Setup Instructions

### Prerequisites

- Java 8+
- Maven

### IntelliJ

1. File → New → Project from Existing Sources
2. Select project folder
3. Import as Maven

### Run

```bash
mvn compile
mvn test
mvn exec:java -Dexec.mainClass="com.drone.sim.Main"
