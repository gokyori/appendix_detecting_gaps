## Appendix A

### Example code used in experiment
```java
import java.util.ArrayList;

public class ArrayListEx1 {
    public static void main(String[] args) {

        ArrayList<String> travelList = new ArrayList<String>();

        travelList.add("Switzerland");
        travelList.add("Denmark");
        travelList.add("India");
        travelList.add("China");
        travelList.add("Thailand");
        travelList.add("Bhutan");

        ArrayList<String> newTravelList = new ArrayList<>();
        for (int i = 0; i <= 5; i++) {
            newTravelList.add(i, travelList.get(i));
        }

        newTravelList.remove("China");
        newTravelList.remove(0);

        System.out.print(newTravelList);
    }
}
```

### Expert Explanation
The program creates a person’s original travel list, creates a new travel list from the original, and then modifies the
new travel list. Make an arrayList travelList for holdjng the travel list and add destinations(countries) to the travel
list. Declare an arrayList travelList whose elements are of type String and add Switzerland, Denmark, India, China,
Thailand, and Bhutan. Creates an arrayList named travelList. Create a list newTravelList from the original travel list
travelList. Create an arrayList newTravelList for copying new travel destinations. The element of the arrayList are
of types string. The array element Switzerland, Denmark, India, China, Thailand and Bhutan are added to arrayList.
Create a for loop that runs from index i= 0 to i= 5 .Get elements of arrayList travelList at position i and add the
element to arrayList newTravelList at index position i. Remove an element from newTravelList and print the values
of newTravelList. Remove China from newTravelList and remove element at index 0. The value printed is [Denmark,
India, Thailand, Bhutan].

### Expert Explanation with Minor Issues (distorted)
The program creates a person’s original travel list, creates a new travel list from the original, and then modifies the
new travel list. Create an arrayList travelList for holding the travel list and add destinations(countries) to the travel
list. Declare an arrayList travelList whose elements are of type String and add Switzerland, Denmark, India, China,
Thailand, and Bhutan. Creates an arrayList named travelList. Create a list newTravelList from the original travel list
travelList. Create an arrayList newTravelList for copying new travel destinations. The element of the arrayList are
of type string. The array element Switzerland, Denmark, India, China, Thailand and Bhutan are added to arrayList.
Create a for loop that runs from index i= 0 to i= 5 .Get elements of arrayList travelList at position i and add the
element to arrayList newTravelList at index position i. Remove an element from newTravelList and print the values
of newTravelList. Remove China from newTravelList and remove element at index 0. The value printed is [Denmark,
India, Thailand, Bhutan].


### Incomplete Explanation
Declare an arrayList travelList whose elements are of type String and add Switzerland, Denmark, India, China, Thai-
land, and Bhutan. Creates an arrayList named travelList Adds Swizerland to arrayList travelList Create a list newTrav-
elList from the original travel list travelList. Create an arrayList newTravelList for holding new travel destinations. The
element of the arrayList are of type string. The element Switzerland, Denmark, India, China, and Thailand are added
to arrayList. Gets element of arrayList travelList at position i and add the element to arrayList newTravelList at index
position i Remove an element from newTravelList and print the values of newTravelList. Remove China from new-
TravelList and remove element at index 0. Removes China from arrayList newTravelList Removes element of arrayList
newTravelList at index position 0. The value printed is [Denmark, India, Thailand].

### Error Injected Code

```java
import java.util.ArrayList;
public class ArrayListEx1 {
    public static void main(String[] args) {
        
        ArrayList < String > travelList = new ArrayList < String > ();
        
        travelList.add("Switzerland");
        travelList.add("Denmark");
        travelList.add("India");
        travelList.add("China");
        travelList.add("Thailand");
        travelList.add("Bhutan");
        
        ArrayList < String > newTravelList = new ArrayList <  > ();
        for (int i = 0; i < 5; i++) {
            
            newTravelList.add(i, travelList.get(i));
        }
        
        
        newTravelList.remove("China");
        
        newTravelList.remove(0);
        System.out.print(newTravelList);
    }
}
```


### Incorrect Explanation from the Error Injected Code

The program creates a person’s original travel list, creates a new travel list from the original, and then modifies the new
travel list. Make an arrayList travelList for holdjng the travel list and add destinations(countries) to the travel list. De-
clare an arrayList travelList whose elements are of type String and add Switzerland, Denmark, India, China, Thailand,
and Bhutan. Creates an arrayList named travelList. Create a list newTravelList from the original travel list travelList.
Create an arrayList newTravelList for copying new travel destinations. The element of the arrayList are of types string.
The array element Switzerland, Denmark, India, China and Thailand are added to arrayList. Create a for loop that runs
from index i= 0 to i ¡ 5 .Get elements of arrayList, travelList at position i and add the element to arrayList newTravelList
at index position i. Remove an element from newTravelList and print the values of newTravelList. Remove China from
newTravelList and remove element at index 0. The value printed is [Denmark, India, Thailand].



## Appendix B: 

## Case Study: Feedbacks Generated by LLMs

### Case Study 1

***Benchmark:*** The explanations are complete and correct. Good Job!


***Prompt P2 (LLama3):*** The explanation is mostly correct but it has some redundant and unclear parts. The explanation is mostly correct, but it’s missing a crucial detail. The line for (int i = 0; i ¡= 5; i++) should be for (int i = 0; i ¡
travelList.size(); i++) to ensure that the loop runs for the actual number of elements in the travelList ArrayList, rather than hardcoding the value 5.

***Few-shot (LLama3):*** The explanation is correct, but it’s missing a crucial detail. The for loop in the code iterates from 0 to 5, but the explanation doesn’t mention the purpose of this loop, which is to copy the elements from the original travelList to the newTravelList. Here’s the corrected explanation: ”The program creates a person’s original travel list, creates a new travel list from the original by copying elements using a for loop, and then modifies the new travel list.”Or, in other words, the explanation doesn’t explicitly state that the loop is used to populate the newTravelList.

***Fine-Tune (LLama3):*** The explanations are complete and correct. Only some minor typos or some other minor issues.
Impressive! Only some minor typos or some other minor issues. Only some minor typos or some other minor issues.
Impressive. . . . . . . . . . . . . . . . . . . . . . . . Everything is perfect. Only some minor issues. Just some minor typos. Only one
minor typo. Very Good. Only one small typo. Just a single typo. Only a few minor issues. Only a few typos. Only two
minor typos. Just two typos. Not at all. So Impressive. Only some minor corrections. Only a few minor errors. Fine. No
issues. All are correct. Wonderful. Exactly Correct. All Good. Perfect.

***Preference Alignment (LLama3):*** The explanations are complete and correct. Great work!!


### Case study 2

***Benchmark:*** The explanations is incomplete. The following lines are missing. “ The program creates a person’s original travel list, creates a new travel list from the original, and then modifies the new travel list. Create an arrayList travelList for holding the travel list. Add destinations(countries) to the travel list. “ 

***Prompt P1 (Mistral):*** The explanation is complete and correct, great job! However, I would like to suggest a few minor improvements: Instead of repeating the same information, you could rephrase some sentences to improve clarity. You could mention that the for loop is used to copy elements from travelList to newTravelList. 

***Prompt P2 (Mistral):*** The explanation is mostly correct, but it’s missing a crucial detail: the reason why ”Switzerland” is not in the final output. The code removes the element at index 0, which is ”Switzerland”, so it’s not included in the final list. Great job! The explanation is almost perfect, just missing a small detail about the removal of ”Switzerland”. 


***Few-shot (Mistral):*** The explanation is correct, but it can be improved for clarity and completeness. Here’s a specific point that was missing in the original explanation: The reason why ”Denmark” is now at index 0 in newTravelList after removing ”Switzerland” (the original element at index 0). 



***Fine-Tune (Mistral):*** The explanation is incomplete. The explanation is missing details about the loop that copies elements from travelList to newTravelList. The loop runs from 0 to 5, which corresponds to the indexes of the elements being copied. 



***Preference Alignment (Mistral):*** The explanation is incomplete. The explanation is missing the summary of the code. “The following line is missing: The program creates a person’s original travel list, copies it to a new list, and then modifies the new list. Positive Feedback: Good job on the explanation”







