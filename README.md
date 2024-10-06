Name: Dawid Biel
UIN: 665470421

HW 1 Cloud Computing
This ia a program for parallel distributed processing of a large corpus of text.

Installation:
Java JDK 8 or Higher, Apache Hadoop, sbt, IntelliJ IDEA, SCALA

Steps:
Clone repository

git clone git@github.com:djbiel2/CS441HW1.git
cd CS441HW1

Make sure all the dependencies are installed
stb compile

Setup the Hadoop cluster on AWS EMR

Edit the application.conf to your specific configurations. 
-trainer is for the word to vector model
-main is the paths 
-sliding_window Parameters to the sliding window

Running the program

curl -L https://www.scala-sbt.org/sbt-rpm.repo | sudo tee /etc/yum.repos.d/sbt.repo
sudo yum install sbt -y
sbt sbtVersion
sudo yum install java-11-amazon-corretto -y
java -version
cd ~/CS441HW1




sbt "runMain Main"


Upload it to aws
