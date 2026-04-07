# JS-Assignment

## Fundamentals of Web Design – Assignment 4

This repository contains my solutions for Assignment 4 of FWD (CSE 106).
All the questions are done using basic JavaScript only, as taught in class.

I have used `prompt()` to take input and `alert()` to show output, as mentioned in the assignment instructions.

Each question is written in a separate file.

---

## Question 1: Digit Gatekeeper

**Approach:**

In this question, I looped from L to R and checked each number.
First I checked if it is divisible by K. Then I calculated sum of digits using a loop.
I also made sure that the number does not contain 0.
After that I checked if the sum is prime using a helper function.

If all conditions are satisfied, I increase the count.

**Time Complexity:**
Roughly O(R - L)

---

## Question 2: Roll-Seed Lock

**Approach:**

Here I started with N and repeated the process 3 times using a loop.
If the number is even, I divided it by 2 and added seed.
If it is odd, I multiplied by 3 and subtracted seed.

After 3 steps, I checked:

* if number is 3 digit
* if middle digit is equal to seed

Based on that, I printed YES or NO.

**Time Complexity:**
O(1)

---

## Question 3: Mirror Corridor

**Approach:**

I used a loop from 0 to 100000 for X.
For each X, I calculated N + X and checked two things:

* if it is divisible by K
* if it is palindrome

For palindrome, I converted number to string and reversed it.

The first X that satisfies both conditions is printed.

If nothing found, print -1.

**Time Complexity:**
Around O(100000)

---

## Question 4: Fare Calculator

**Approach:**

I followed the steps given in question one by one.

* First calculated base fare
* Added 20 if late
* Added 10% if distance > 10
* Then adjusted using seed (add or subtract)
* Finally rounded it to nearest multiple of 5 using Math.ceil

**Time Complexity:**
O(1)

---

## Question 5: Skipping Numbers

**Approach:**

In this question, I kept increasing m from 1.
For each number, I checked if it is divisible by (seed + 2).
If not divisible, I added it to sum.

I stopped when sum became greater than or equal to N.

Then I printed m and sum.

(Note: I followed the condition sum ≥ N strictly.)

**Time Complexity:**
Depends on m (linear)

---

## Question 6: Contest Score Judge

**Approach:**

I calculated score using given formula:
score = 3a + b - 2c

Then:

* if score < 0, set it to 0
* if total submissions > 50, subtract 10

Finally checked:

* score ≥ 60 → PASS
* otherwise → FAIL

**Time Complexity:**
O(1)

---

## Notes

* I have not used any advanced concepts
* Only loops, conditions, and basic JS
* No hardcoding is done
* Each question is in separate file as required

---

## How to Run

Open the HTML file in browser (Chrome recommended).
It will show prompt for input and alert for output.

---
