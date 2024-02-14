__Part 1 - Bugs__
- *Includes failure inducing input*
  - <pre>
    public void testReverseInPlace2() {
    int[] input2 = {1, 2, 3};
    ArrayExamples.reverseInPlace(input2);
    assertArrayEquals(new int[]{3, 2, 1}, input2);
    }
  </pre>
  
- *Does NOT include failure inducing input*
  - <pre>
    public void testReverseInPlace() {
    int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3 }, input1);
	}
  </pre>
  
- *Code causing failure inducing input*
  - <pre>
    static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
     }
    }
  </pre>

- *Symptom for failure inducing input from above code*
  - ![Image](JunitFailReverseinPlace.png)
 
- *Code that DOES NOT cause failure inducing input*
  - ![Image](JunitPassReverseinPlace.png)
 
__Part 2 - Researching Commands__
- I chose the `find` command
  - `type` command line option
    - This command line option determines what kind of files are in specific directories. For example, the command `find path -type f` looks for all the elements in the path and f tells it to look for elements that are files. Similarly, the command `find path -type d` looks for all the elements in the path but d tell it to look for elements that are directories and prints them out. 
    - *Example 1*
    - ```
      Jeffu@Jeff MINGW64 ~/docsearch (main)
      $ find technical/biomed/ -type f
      technical/biomed/1468-6708-3-1.txt
      technical/biomed/1468-6708-3-10.txt
      technical/biomed/1468-6708-3-3.txt
      technical/biomed/1468-6708-3-4.txt
      technical/biomed/1468-6708-3-7.txt
      technical/biomed/1471-2091-2-10.txt
      technical/biomed/1471-2091-2-11.txt
      ... OMITTING 100+ files ...
      ```
    - This output prints out all the file type files in the biomed directory. (Because the biomed directory have so many files, only the first few are shown.)
    - *Example 2*
    - ```
      Jeffu@Jeff MINGW64 ~/docsearch (main)
      $ find technical/ -type d
      technical/
      technical/911report
      technical/biomed
      technical/government
      technical/government/About_LSC
      technical/government/Alcohol_Problems
      technical/government/Env_Prot_Agen
      technical/government/Gen_Account_Office
      technical/government/Media
      technical/government/Post_Rate_Comm
      technical/plos
      ```
    - This output prints out all the files that are directories in the technical directory.
    - This command line option is useful because when were dealing with large directories, we can identify all the elements that are files or directories to better understand the large directory as a whole. The source that I used for this command line option is this <a href="https://www.geeksforgeeks.org/find-command-in-linux-with-examples">Webpage</a>

  
