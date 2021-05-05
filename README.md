<!-- INTRODUCTION -->
<br />
<p align="center">
    <img src="https://user-images.githubusercontent.com/42817904/117049270-38461400-ad14-11eb-97e8-ddc5c280ed77.png"/>
  <h2 align="center">SCRUM UP</h2>
  <p align="center">
    A student approach to software development project management tools.
    <br />
    <a href="https://drive.google.com/file/d/1h2cLj1pzEAhUC4m7TYT2P2HXZQH1-rGA/view?usp=sharing"><strong>Explore the project report »</strong></a>
    <a href="https://drive.google.com/file/d/1-lVEbOgG-SKqOaqZsePi81gwF9fyLYex/view?usp=sharing"><strong>Explore the user manual »</strong></a>
    <br />
  </p>
</p>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

Scrum is a lightweight, iterative and incremental framework for managing complex work. 

This particular framework is recommended to be used by the 2nd Semester students at VIA University College in Horsens, Denmark.

Key features of SCRUM are that core-architecture elements of the system are being released through iterations (Sprints) and that the team is flexible and customer-oriented being able to bring alterations to the system through each iteration. 


<strong>Features:</strong>
* Provide roles creation and privileges: Each user has a certain role and a certain degree of authority and credentials in the system. 
* Provide planning tools: Users are able to plan and document each of their iterations 
* Remote functionality: Users are able to use the system remotely.

### Built With

* [Java JDK 1.8](https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html)
* jdbc - Java Database Connectivity
* [JavaFX Scene Builder](https://gluonhq.com/products/scene-builder/) - GUI
* [ASP .NET Core](https://dotnet.microsoft.com/download) - Web APIs
* [Entity Framework Core + SQLite](https://docs.microsoft.com/en-us/ef/core/) - Database

<!-- GETTING STARTED -->
## Getting Started

Code is located in `Code/src` folder. 

Documentation is located in `documentation` folder. SCRUM and UP framework related things are in `Analysis and Design` folder.

### Prerequisites

* [Java JDK 1.8](https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html)
* Java IDE

### Installation

1. Clone the repository:
  ```
 git clone https://github.com/davele-itsme/Semester-project-2.git
  ```
2. Open the project in Java IDE
3. Run: RunApplicationHQ, RunApplicationWH, RunApplicationRT

If you want to create tables with already existing data to test the system, please follow these guidelines

#### Set up tables:
1. Open PgAdmin
2. Create a new database
3. Go into src/jdbc/ and open DataBaseModel
4. Find setConnection() and change the Strings to match the database
5. Run src/jdbc/Setup.java

Now you have the required tables and dummy data


Now you have to run the server before running the applications
Run application:
1. Run src/network/Server/Server.java
2. Open src/Run.java, src/RunHQ.java and src/RunRT.java and change the HOST String to "localhost"

Now you can use RunApplicationHQ, RunApplicationWH and RunApplicationRT to open the different clients.
Beware of closing clients, our Server still thinks you're connected and will keep throwing exceptions, slowing down your system. 


