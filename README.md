PluralSight JUnit5 Notes
1) Tests are used to check target code instead of the whole system
2) Tests are used to check if a code execution is done correctly with desired outputs
3) Test checks use expected outputs and actual outputs for testing
4) Tests can be used on an incomplete system or project if the target code is done
5) Tests help show if the target code can be invoked in the program
6) Tests can be used as a reference for a target code's purpose
7) Intellij has a test class shortcut that can create a test class
8) @Test annotation is used to let intellij know the code is a test
9) When using assertEquals() first argument is always expected output, second is always actual output
10) assertSame() is used to see if the given arguments point to the same object, assertNotSame() is used for the opposite
11) assertIterableEquals() used to compare iterable objects given, iterables return objects for use in a for loop
12) Annotations of note-
    @BeforeEach: runs annotated method once before each test
    @BeforeAll: runs annotated method once before all tests
    @AfterEach: runs annotated method once after each test
    @AfterAll: runs annotated method once after all test methods
13) @AfterAll and @BeforeAll should be static as they operate on class level
14) assertMethods() allow for a String message as a third argument that prints when a test fails
15) @DisplayName(String) can be used to rename the displayed method names in the Test Results window
16) @Nested annotation can be used to nest test methods within a test class
17) @Disabled annotation can be used to ignore a test method when testing a whole class
18) JUnit Assertions are short-circuit / they are terminated on the first failed check
19) assertAll() can be used to prevent short-circuiting withing a test method by taking in assertMethods() as parameters
20) All assertMethods() within an assertAll() must be a lambda expression / (parameters if any/bank if none) -> used to make a method/parameter anonymous
21) @Tag(String) annotation can be used to tag methods to be executed as a group
22) Run/Debug Configuration window can be used to execute tests of a given tag value
23) Single Responsibility Principle: a unit of code does one thing
24) Extract Method can be used to rename and copy a target method to access it easier
25) Test Double can be created to satisfy a code's exterior dependency when testing
26) Test-driven Development is described by stating what a test should do, then implement the described feature, then return to the test for the next function