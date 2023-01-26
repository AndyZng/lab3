Part 1: 
<img width="921" alt="image" src="https://user-images.githubusercontent.com/115373033/214974176-55d2dd9b-f522-462c-8887-3ac6e7a4ab57.png">

<img width="960" alt="image" src="https://user-images.githubusercontent.com/115373033/214974421-911fa13d-a581-4a70-a90b-c61a97b67474.png">

<img width="379" alt="image" src="https://user-images.githubusercontent.com/115373033/214974453-1bdb502b-a874-4153-81bf-bf00e8bb4f81.png">


Bug Testing
---


Original Code for reverseInPlace:

<img width="336" alt="image" src="https://user-images.githubusercontent.com/115373033/214964115-27492f9a-d71c-4289-a429-78538312c95c.png">

ReverseInPlace tests:
The original two tests passed, but there was an incorrect output in the third test which tested an array longer than 1.
The first two tests do not induce failure since they test arrays with lengths 1 or less.
<img width="731" alt="image" src="https://user-images.githubusercontent.com/115373033/214963704-78658f21-03d1-4c09-937f-515ec17c1d10.png">

Symptom:
The problem with this code is that the array changes itself as it iterates backwards. 
![image](https://user-images.githubusercontent.com/115373033/214967881-e362cad1-cecb-4f23-a4a3-79f841ccdbb2.png)

Bug: The last term and first term are the same
<img width="298" alt="image" src="https://user-images.githubusercontent.com/115373033/214968094-b0e38d80-4952-4d1b-9135-97d06c4ef2d0.png">
Fix: By creating a hard copy of the array we want to reverse, and then iterating through it backwards, we can get our desired result. 
<img width="352" alt="image" src="https://user-images.githubusercontent.com/115373033/214968189-8be9fb5b-b939-4591-b0aa-62380a31eff6.png">

What I learned:

I learned how to test and debug my code by using JUnit to write tests and see how my outputs differed from my desired inputs. I also learned how to create a solution
for my bugs. 







