Unity Target Shooting Game - Readme
Overview
This repository contains the scripts for a simple target shooting game developed in Unity. The game involves shooting and destroying targets to earn points. It features different difficulty levels and a basic UI.

Scripts
GameManager.cs
Description: GameManager.cs is responsible for managing the game's logic and UI.

Key Functions and Variables:

public List<GameObject> targets: A list of target objects.
public TextMeshProUGUI scoreText: Text element for displaying the player's score.
public TextMeshProUGUI gameOverText: Text element for displaying the game over message.
public bool isGameOver: A boolean flag to track whether the game is over.
public Button restartButton: A button for restarting the game.
public GameObject titleScreen: The game's title screen GameObject.
private float spawnRate: Controls the spawn rate of targets.
private int score: Stores the player's score.
Functionality:

Manages game flow, including game over, score updates, and game restart.
Spawns targets at random intervals.
Controls difficulty levels.
DifficultyButton.cs
Description: DifficultyButton.cs sets the difficulty level when a button is clicked.

Key Functions and Variables:

public int difficulty: The difficulty level associated with the button.
Functionality:

Sets the game difficulty level when the button is clicked.
Target.cs
Description: Target.cs defines the behavior of individual target objects.

Key Functions and Variables:

private Rigidbody targetRb: The target's Rigidbody component.
private GameManager gameManager: Reference to the game manager.
private float minSpeed: Minimum speed at which targets move.
private float maxSpeed: Maximum speed at which targets move.
private float maxTorque: Maximum torque applied to targets.
private float xRange: Horizontal range within which targets spawn.
private float ySpawnPos: Y-position at which targets spawn.
public int pointValue: Points awarded for hitting the target.
public ParticleSystem explosionParticle: Particle system for target destruction.
Functionality:

Initializes target movement, position, and torque.
Handles mouse click events to destroy targets.
Detects collisions with other objects and triggers game over if necessary.
How to Use
Import the provided script files into your Unity project.

Attach the scripts to relevant GameObjects in your scene.

Customize the game's appearance and behavior using Unity's Inspector.

Run the game in the Unity editor or build and deploy it to your desired platform.

Contributing
Feel free to contribute to the project by enhancing the gameplay, adding new features, or improving the codebase.

License
This project is licensed under the MIT License. See the LICENSE file for details.
