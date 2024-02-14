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
