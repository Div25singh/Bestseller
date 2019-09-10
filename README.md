# Bestseller

This Project mainly focuses on a Book Club that sells fine books to customers all over the world. Each time a book is sold the Book-Number, the Number-of-Copies and a one-character field indicating the Sale-Status (Normal Sale, Free Gift, Reduced Price (N, F, R)) is written to a Book-Sales-File. 
A program is required to print a list of the ten bestselling books (by copies sold) in the Book Club from the Book-Sales-File. Only Normal Sale books should be considered. 
It’s like a book recommendation system that tells the customers about the Bestselling books

PROBLEM STATEMENT 
"Bestselling" refers to the estimated number of copies sold of each book, rather than the number of books printed or currently owned. The books are listed according to the highest sales estimate as reported in reliable, independent sources. 
Number of Files Used 
 Book Master File 
The Book Master File is a sequential file sequenced on ascending Book-Number. The records have the following description; 
FIELD TYPE LENGTH VALUE Book-Number 9 5 00001-99999 Book-Title X 25 - Author-Name X 25 - 
  
 Book Sales File 
The Book Sales File is not in any particular sequence but we are guaranteed that a Book-Number that occurs in the file will have a corresponding entry in the Book Master File. 
FIELD TYPE LENGTH VALUE Book-Number 9 5 00001-99999 Number-Of-Copies 9 2 1-99 Sale-Status X 1 N,F,R 
 
 
 OBJECTIVE 
The program will sort the Book Sales file throwing away unwanted records (F, R). Then accumulate the sales for a book. If the book is in the top ten, then get the BookTitle and Author-Name from the Book Master File. When the Sorted Book Sales File has been processed, print out the top ten best sellers. 
