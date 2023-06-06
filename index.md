# Lab Report 5
## Part 1: Debugging
**What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?**
* The environment that I am currently using is a Macbook Pro 2020 on Visual Studio Code. I'm trying to run my `buglab.java` file from my terminal, which also includes a bash script called `error.sh`.

**Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.**
* The symptom I'm seeing right now is that my file is compliing, but when I try to run it, there seems to be an error within my code that isn't outputing the right result.
```
veraniasalcidodale@Favorites-MacBook-Pro labreport5 % java buglab
Exception in thread "main" java.lang.ArithmeticException: / by zero
        at buglab.main(buglab.java:7)
```

**Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.**
* The failure-inducing context would be my actual my buglab.java file:
```
public class buglab 
{
    public static void main(String[] args) {
        int x = 5;
        int y = 0;
        
        int result = x / y;
        
        System.out.println("Result: " + result);
    }
}
```

## Part 2: Reflection
*
