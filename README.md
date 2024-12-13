# PeopleYouMayKnow
# People You May Know

## Table of Contents

1. [Overview](#overview)
2. [Features](#features)
3. [Project Setup](#project-setup)
    - [Prerequisites](#prerequisites)
    - [Installing](#installing)
    - [Running the Project](#running-the-project)
4. [Algorithm Details](#algorithm-details)
5. [Sample Data Format](#sample-data-format)
6. [How to Contribute](#how-to-contribute)
7. [Acknowledgements](#acknowledgements)

## Overview

The **People You May Know** algorithm recommends potential connections (friends) on social media platforms based on mutual interests, hobbies, and shared connections. This project implements the algorithm in Java using graph-based data structures, such as HashMaps and graphs, to map users to their common friends and interests. The goal is to predict which users are likely to be connected, helping social media platforms to suggest new friends for users.

This project was developed as part of a **Project-Based Learning (PBL)** initiative and won second place at the PBL open day event.

## Features

- **Graph Representation:** Users are represented as nodes, with friendships and connections as edges in an undirected graph.
- **Mutual Interests:** The algorithm analyzes common hobbies or interests shared between users to improve connection suggestions.
- **Friend Recommendation:** The algorithm generates potential friend recommendations based on mutual friends and shared interests.
- **Java Implementation:** The project is written in Java, utilizing core concepts and data structures like HashMaps and Graphs.

## Project Setup

### Prerequisites

To run this project, you'll need:

- **Java 8 or higher**
- **Basic knowledge of Graph Theory and Algorithms**

### Installing

Clone the repository:
```bash
git clone https://github.com/username/people-you-may-know.git
cd people-you-may-know

### Running the Project

If you have the project in a single file, run it by compiling and executing the Java file:

```bash
javac PeopleYouMayKnow.java
java PeopleYouMayKnow
## Algorithm Details

1. **Graph Representation:**
   - Users are represented as nodes.
   - Friendships are undirected edges connecting users.
   - Mutual interests are stored as attributes in the user (node), represented using HashMaps.

2. **Recommendation Logic:**
   - For each user, the algorithm checks their direct friends (edges).
   - For each friend, the algorithm looks for mutual friends and shared attributes (interests).
   - The system suggests users who share a higher number of mutual connections or common interests.

3. **Time Complexity:**
   - The time complexity of the recommendation algorithm is O(V + E), where V is the number of users (nodes) and E is the number of friendships (edges).

## Sample Data Format

To test the algorithm, the sample user data might look like this:

User1: [Music, Hiking], Friends: [User2, User3] <br>User2: [Music, Cooking], Friends: [User1, User4] <br>User3: [Hiking, Reading], Friends: [User1, User5] <br>User4: [Cooking, Reading], Friends: [User2] <br>User5: [Reading, Hiking], Friends: [User3]<br>

- **Interests** are listed as a comma-separated list of hobbies.
- **Friends** are listed by usernames, indicating the user's connections.

You can add this data into a text file or hard-code it in the `PeopleYouMayKnow` Java class for testing purposes.

## How to Contribute

1. Fork the repository.
2. Clone your fork to your local machine.
3. Create a new branch (`git checkout -b feature-name`).
4. Make your changes and commit them (`git commit -am 'Add new feature'`).
5. Push to the branch (`git push origin feature-name`).
6. Create a pull request.

## Acknowledgements

- This project was inspired by real-world algorithms used in social media platforms for friend recommendations.
- Special thanks to the Project-Based Learning team for their support and guidance.

