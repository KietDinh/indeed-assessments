## Software Developer

#### Q1. Complete the function shown below by replacing // INSERT MISSING CODE with the correct line of code. Language: C

    ```
        // copy a string from the original to the destination
        // and return the number of characters copied
        int mystrcpy(char *destination, char *original) {
            int count = 0;
            while (*original != '\0') {
                *destination++ = *original++;
                // INSERT MISSING CODE
            }
            *destination = *original;
            return count;
        }
    ```

- [ ] original++;
- [x] count++;
- [ ] destination++;

#### Q2. Threads allow a developer to .

- [ ] have tasks to completed in the correct order
- [x] perform tasks in parallel
- [ ] deploy only certain modules of an application
- [ ] reduce the resources needed for an application
- [ ] build a less complex application

#### Q3. Which process requires automated builds and testing to verify software during development?

- [x] Continuous integration
- [ ] System integration
- [ ] Agile methodology
- [ ] Deployment integration
- [ ] Integration tests

#### Q4. You have two microservices that need to communicate with each other without holding up a thread on either end. One service will receive an ID and return a message once the job is complete. Which communication framework should be used?

- [ ] Create a third service to handle the interaction between the services
- [ ] Have a shared database that allows both applications to read and write to the tables to share the data instead of having to communicate
- [x] Use a RESTful architecture for both, send the ID through a POST, and ping the service with a GET until a response is available
- [ ] Use asynchronous messaging to send and receive messages between each microservice
- [ ] Abandon the microservice architecture so no interaction is needed

#### Q5. What's the value of result after the loop completes? Language: Java

    ```
        int[] numbers = new int[]{1, 2, 3, 4};
        int result = 0;
        for (int number : numbers) {
            result *= number
        }
    ```

- [x] 0
- [ ] 4
- [ ] 6
- [ ] 10
- [ ] 24

#### Q6. Complete the function shown below by replacing # INSERT MISSING CODE with the correct line of code. Language: Python

    ```
        # find the count of odd numbers and
        # the smallest odd number in a list
        def get_smallest_odd(numlist):
            oddcount = 0
            smallest = float('inf')
            for num in numlist:
                if (num % 2) != 0:
                    oddcount += 1
                    if num < smallest:
                        # INSERT MISSING CODE
            return oddcount, smallest
    ```

- [ ] break
- [x] smallest = num
- [ ] num = smallest
- [ ] smallest = smallest + 1
- [ ] smallest = oddcount

#### Q7. What's wrong with this code? Language: Java

    ```
        public int doThings(String numberString) {
            try {
                int i = Integer.parseInt(numberString);
            } catch(Exception e) {
                System.out.println(e);
            }
            return i;
        }
    ```

- [ ] numberString should be null checked
- [ ] Nothing's wrong
- [x] i isn't in scope to be returned
- [ ] Integer can't cast to int
- [ ] parseInt() can't produce Exception

#### Q8. What does this method return? Language: Java

    ```
        public List<Integer> someFunction(final List<Integer> numbers) {
            List<Integer> result = new ArrayList<Integer>();
            for (int i = numbers.size() - 1; i >= 0; i--) {
                result.add(numbers.get(i));
            }
            return result;
        }
    ```

- [ ] An incrementally sorted list
- [ ] A decrementally sorted list
- [ ] Throws ArrayIndexOutOfBoundsException
- [x] A reverse ordered list
- [ ] The same list

#### Q9. Complete the function shown below by replacing // INSERT MISSING CODE with the correct line of code. Language: JavaScript

    ```
        function findLargestIndex(theArray) {
            index = 0;
            largestValue = theArray[0];
            for (i = 0; i < theArray.length; i++) {
                if (theArray[i] > largestValue) {
                    index = i;
                    // INSERT MISSING CODE
                }
            }
            return index;
        }
    ```

- [x] largestValue = theArray[i];
- [ ] continue;
- [ ] i = largestValue;
- [ ] largestValue = i;
- [ ] break;

#### Q10. What does the function someFunction() perform? Language: Java

    ```
        public Node someFunction(Node root, int key) {
            if (root == null || root.key == key) {
                return root;
            }

            if (root.key > key) {
                return someFunction(root.left, key)
            }

            return someFunction(root.right, key)
        }
    ```

- [x] Searches through a binary tree for a value
- [ ] Checks to find null values in a binary tree
- [ ] Sorts values of a binary tree
- [ ] Builds out a binary tree
- [ ] Throws an uncaught exception on all calls

#### Q11. Is there anything wrong with this code? Language: Java

    ```
        int[] merge(int[] a, int[] b) {
            int[] result = new int[a.length + b.length];
            for(int i = 0; i< a.length; i++) {
                result[2*i] = a[i];
                result[(2*i)+1] = b[i];
            }
            return result;
        }
    ```

- [ ] Yes; the code runs, but doesn't merge the two arrays
- [x] Yes; the code merges the arrays, but only if they're the same length
- [ ] Yes; the code doesn't compile
- [ ] Yes; the code uses variables to set the size of the array
- [ ] No; the code functions as intended

#### Q12. Which input would return a value of true? Language: Java

    ```
        public boolean isSpecial(String text) {
            String tempText = alterText(text);
            return text.equals(tempText);
        }

        public String alterText(String inputText) {
            if(inputText == null || inputText.isEmpty()) {
                return inputText;
            }
            return inputText.charAt(inputText.length() - 1) + alterText(inputText.substring(0, inpuText.length() - 1));
        }
    ```

- [x] "ab1221ba"
- [ ] "aaabbb"
- [ ] "abcdef"
- [ ] "abcd4321"
- [ ] "a1a1b2"
