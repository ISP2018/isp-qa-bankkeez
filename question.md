#Questions

**Q1.** As a beginner developer, you are new to a lot of things, you have a chance to ask an expert a question. You asked him how to become a good developer like you. He answered, **"Don't reinvent the wheel when you can steal it".** What do you think an expert mean according to the choices: 
**(Choose all choices if they are all correct)**

(One of correct choice): As a beginner developer, you'll find the problem that that you're trying to solve that has already been solved by somebody else. Design patterns are generic solution. So as framework that extends those pattern for simplifying your application.

Reference: https://softwareengineering.stackexchange.com/questions/34173/are-there-concrete-reasons-not-to-use-libraries-and-code-snippets-heavily

**Q2.** 
``` @Test
public void testDivide(){
double x = 5;
double y = 30000;
assertEquals(0.00016666666666666,5/30000);
}
```
Is the code correct or is it wrong? If correct leave the answer balnk or else fix the code correctly.

Answer: 
``` 
static final double TOL = 1.0E-5;
@Test
public void testDivide(){
double x = 5;
double y = 30000;
double expected = 0.00016666666666666;
assertEquals(expected,x/y,TOL);
}
```

**Q.3** You have a java project called unitlabtest in github. In your first commit, you accidentally push **.classpath** and **.project** file. You delete the file manually through the github website. Afterthat you continue your work and now your pushing the second commit. What problem is found and how can this be fix?

Sequence of commits between your local version of the branch and the remote version isn't linear, then the push will be rejected (**non-fast-forward**). This can be fix easily by using command git pull  the git push by later on.

**Q.4** As a good developer you must be expert at debugging. Debugging will let you step through your program, jumping deeper into the lower layers and learning what really happens when you call a method, or set a value, or make a network request. Imagine you're working on an ATM program. You are at the money withdrawn part. You found many bugs while working on the part. How can you solve the problem? State atleast one way and explain.

1. For java, using JUnit, create test cases to test all the method for all possible outcomes.

2. According to [PAD](https://media.pragprog.com/titles/pad/PAD-pulloutcard.pdf) agile developer: Tip 25 **"Write code to be clear not clever"**.

3.According to [PAD](https://media.pragprog.com/titles/pad/PAD-pulloutcard.pdf) agile developer: Tip 28 **"Write code in short/edit/build/test cycles"**.











