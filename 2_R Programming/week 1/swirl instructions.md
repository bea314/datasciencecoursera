# Swirl instructions

## 1. Install swirl
install.packages("swirl")  
packageVersion("swirl")

## 2. Load swirl
library(swirl)  
rm(list=ls())

## 3. Install the R Progroamming course
install_from_swirl("R Programming")

## 4. Start swirl and complete the lessons
swirl()

## 5. Commands

| When you are at the R prompt (>):
| -- Typing skip() allows you to skip the current question.
| -- Typing play() lets you experiment with R on your own; swirl will ignore what
| you do...
| -- UNTIL you type nxt() which will regain swirl's attention.
| -- Typing bye() causes swirl to exit. Your progress will be saved.
| -- Typing main() returns you to swirl's main menu.
| -- Typing info() displays these options again.
