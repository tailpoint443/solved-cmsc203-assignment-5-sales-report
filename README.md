Download Link: https://assignmentchef.com/product/solved-cmsc203-assignment-5-sales-report
<br>
Minnie and Mickey are getting ready to send out Holiday bonuses to their hard working employees in Retail District #5. The bonuses are calculated based on how much each retail store sold in each category. The retail store with the highest amount sold in a category will receive $5,000. The retail store with the lowest amount sold in a category will receive $1,000. All other retail stores in district #5 will receive $2,000. If a retail store didn’t sale anything in a category, or they have a negative sales amount, they are not eligible for a bonus in that category. If only one retail store sold items in a category, they are eligible to receive only the bonus of $5000 for that category.

<table width="100%">

 <tbody>

  <tr>

   <td><strong>Assignment Description</strong></td>

  </tr>

 </tbody>

</table>




Create a utility class that manipulates a <strong>two-dimensional</strong> ragged array of doubles. This utility class will be used to create a Sales Report for Retail District #5. It will accommodate positive and negative numbers. Follow the Javadoc provided.

Create a utility class that will calculate holiday bonuses given a ragged array of doubles which represent the sales for each store in each category. It will also take in bonus amount for the store with the highest sales in a category, the bonus amount for the store with the lowest sales in a category and the bonus amount for all other stores.

These utility classes will be used with an existing GUI class to create a sales report and display holiday bonuses.

Testing of these utility classes will be done with the JUnit tests and the GUI class provided for you.

<table width="100%">

 <tbody>

  <tr>

   <td><strong>Concepts tested by this assignment</strong></td>

  </tr>

 </tbody>

</table>
















<ul>

 <li>Creating classes based on Javadoc</li>

 <li>Two Dimensional Ragged Arrays</li>

 <li>Passing arrays to and from methods</li>

 <li>Creating a Utility class (static methods)</li>

 <li>JUnit testing</li>

 <li>Reading from a file</li>

 <li>Writing to a file</li>

 <li>Using methods of the utility class within an existing GUI driver class

  <ul>

   <li>Must follow Javadoc to implement correctly</li>

  </ul></li>

</ul>










<table width="100%">

 <tbody>

  <tr>

   <td><strong>Classes</strong></td>

  </tr>

 </tbody>

</table>




<strong> </strong>




<strong>Utility class </strong><strong>– TwoDimRaggedArrayUtility</strong>

The class <em>TwoDimRaggedArrayUtility</em> will follow the provided Javadoc and will contain the following methods:

<ol>

 <li>Method <strong>readFile </strong>– pass in a file and return a two-dimensional ragged array of doubles</li>

 <li>Method <strong>writeToFile</strong> – pass in a two-dimensional ragged array of doubles and a file, and writes the ragged array into the file. Each row is on a separate line and each double is separated by a space.</li>

 <li>Method <strong>getTotal</strong> – pass in a two-dimensional ragged array of doubles and returns the total of the elements in the array.</li>

 <li>Method <strong>getAverage</strong> – pass in a two-dimensional ragged array of doubles and returns the average of the elements in the array (total/num of elements).</li>

 <li>Method <strong>getRowTotal</strong> – pass in a two-dimensional ragged array of doubles and a row index and returns the total of that row. Row index 0 is the first row in the array.</li>

 <li>Method <strong>getColumnTotal</strong> – pass in a two-dimensional ragged array of doubles and a column index and returns the total of that column. Column index 0 is the first column in the array. If a row doesn’t contain that column, it is not an error, that row will not participate in this method.</li>

 <li>Method <strong>getHighestInRow</strong> – pass in a two-dimensional ragged array of doubles and a row index and returns the largest element in that row. Row index 0 is the first row in the array.</li>

 <li>Method <strong>getHighestInRowIndex</strong> – pass in a two-dimensional ragged array of doubles and a row index and returns the index of the largest element in that row. Row index 0 is the first row in the array.</li>

 <li>Method <strong>getLowestInRow</strong> – a two-dimensional ragged array of doubles and a row index and returns the smallest element in that row. Row index 0 is the first row in the array.</li>

 <li>Method <strong>getLowestInRowIndex</strong> – a two-dimensional ragged array of doubles and a row index and returns the index of the smallest element in that row. Row index 0 is the first row in the array.</li>

 <li>Method <strong>getHighestInColumn</strong> – pass in a two-dimensional ragged array of doubles and a column index and returns the largest element in that column. Column index 0 is the first column in the array. If a row doesn’t contain that column, it is not an error, that row will not participate in this method.</li>

 <li>Method <strong>getHighestInColumnIndex</strong> – pass in a two-dimensional ragged array of doubles and a column index and returns the index of the largest element in that column. Column index 0 is the first column in the array. If a row doesn’t contain that column, it is not an error, that row will not participate in this method.</li>

 <li>Method <strong>getLowestInColumn</strong> – pass in a two-dimensional ragged array of doubles and a column index and returns the smallest element in that column. Column index 0 is the first column in the array. If a row doesn’t contain that column, it is not an error, that row will not participate in this method.</li>

 <li>Method <strong>getLowestInColumnIndex</strong> – pass in a two-dimensional ragged array of doubles and a column index and returns the index of the smallest element in that column. Column index 0 is the first column in the array. If a row doesn’t contain that column, it is not an error, that row will not participate in this method.</li>

 <li>Method <strong>getHighestInArray</strong> – pass in a two-dimensional ragged array of doubles and returns the largest element in the array.</li>

 <li>Method <strong>getLowestInArray</strong> – pass in a two-dimensional ragged array of doubles and returns the smallest element in the array.</li>

</ol>

<strong> </strong>

<strong>Utility class </strong><strong>– HolidayBonus</strong>

The class <em>HolidayBonus</em> will contain the following methods:

<ol>

 <li>Method <strong>calculateHolidayBonus </strong>– pass in a two-dimensional ragged array of doubles, and the bonus amount for the store with the highest sales in a category, the bonus amount for the store with the lowest sales in a category and bonus amount for all other stores. It will return an array of doubles which represents the holiday bonuses for each of the stores in the district. The first entry in the returned array [0] will represent the holiday bonus for the store at [0] in the two-dimensional ragged array of doubles. You will be using methods from the TwoDimRaggedArrayUtility when needed.</li>

 <li>Method <strong>calculateTotalHolidayBonus</strong> – pass in a two-dimensional ragged array of doubles, and the bonus amount for the store with the highest sales in a category, the bonus amount for the store with the lowest sales in a category and bonus amount for all other stores. It will return a double which represents the total of all Holiday Bonuses for the District. You will be using methods from the TwoDimRaggedArrayUtility when needed.</li>

</ol>

<strong> </strong>

<strong>GUI Application </strong><strong>– provided for you</strong>

<ol>

 <li>Uses methods of <em>TwoDimRaggedArrayUtility </em>and<em> HolidayBonus</em></li>

 <li>When the <em>Load Sales Data</em> button is selected the sales data is read from a file and displayed on the screen with the sales data as well as the totals for each store and the totals for each category. The largest sales for each category is highlighted in green. The smallest sales for each category is highlighted in red. The holiday bonus for each store is displayed as well as the total of holiday bonuses.</li>

 <li>The file contains a row for each store and each double in the row is separated by a space</li>

 <li>Student must provide two additional input files and a screenshot of the results of each. Each file will have at least 4 rows and up to 6 numbers on each row. They must represent ragged arrays.</li>

</ol>




<strong>JUnit Test</strong>

<ol>

 <li>Student will implement TwoDimRaggesArrayUtilityTestSTUDENT</li>

 <li>Student will implement HolidayBonusTestSTUDENT</li>

</ol>




<table width="100%">

 <tbody>

  <tr>

   <td><strong>Assignment Details</strong></td>

  </tr>

 </tbody>

</table>

























When GUI application starts (provided), user is shown display of Store Names and Item Names

User selects <em>Load Sales Data</em> to select the file containing the sales data. The application then displays the sales for each store and each item as well as the totals for the store and the totals for the item. The store with the highest sales for each item will be highlighted.

<em>Exit</em> will exit the application.




File Format

The file will be in the following format: one store per line, each sales figure is separated by a space.

<table width="100%">

 <tbody>

  <tr>

   <td><strong>Examples</strong></td>

  </tr>

 </tbody>

</table>




When application starts:




File containing sales data:




Result after selecting Load Sales Data:




File containing sales data (including negative numbers):




Result after selecting Load Sales Data:




File containing sales data (including negative numbers):




Result after selecting Load Sales Data:


