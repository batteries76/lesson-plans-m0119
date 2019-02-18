# Day 02 — HTML & Big O
## Outcomes
Students to have a basic understanding of HTML


## On successful completion of this unit students will be able to:
- construct a HTML page
- link to other HTML pages from the index page
- complete a HTML 5 layout
- create a static web site

## Guided instructions

### HTML
- create a HTML 5 file within a named project folder ```index.html```
- add appropriate meta tags
- open graph tags
- regular HTML tags ```<h1>``` ```<p>``` etc.
- image and media tags
- anchors in pages ```<a>```
- url paths and anchor links
- load in ```index.html``` with server as a static website using ruby
```linux
# http://localhost:3000/
ruby -run -e httpd . -p 3000
```
or
use live reload in vs code
[LiveServer](https://github.com/ritwickdey/vscode-live-server)
- explain difference between unicode (Universal Coded Character Set) and ASCII
- explain utf-8 (Unicode Transformation Format) [Unicode Miracle](https://youtu.be/MijmeoH9LT4)
- page layout & tags (header, nav, main, aside, footer)
- tag attributes
- discuss accessibility
- discuss emmet

### BIG 0
- searching activity
```
Take 12 people up front, as well as 1 person to search, and 1 person to take a tally of search iterations.
```
- what is an algorithm? 
- what is n, what does it represent?

- LINEAR SEARCH
```
- linear search interactive example
Give each a card with an animal name in random order.
```
- discuss randomness (sorted vs unsorted data)
```
Ask a 13th student to find the requested animal from left to right. 
Discuss how many steps (whiteboard)
```
- The average number of steps a linear search takes is explained by n/2.
- explain what 'order of magnitude' is and what 'Big O notation' is
- A linear search is O(n)

- BINARY SEARCH
```
- binary search interactive example
Get the students to sort themselves in alphabetical order.
Ask a new student to move to the center of the students.
Student to choose left or right.
Ask what animal.
If greater, search left, if less than search right.
continue pattern until animal is found
Repeat processes several times to view the different outcomes
```
Discuss how many steps (whiteboard)
- a binary search is O(log n)
- explain what log is.... show values as n increases which can lead to:
- "as n increases, the calculated value (the number of steps taken in the search) increases very very SLOWLY"

- OVER RIDING
- linear search for n=1024 = 1024/2 = 512 steps (on average)
- binary search for n=1024 = log(1024) = 10 steps
- there are different costs associated with each, sorting cost vs searching cost. Binary has a 'set-up' cost of sorting, but then is faster.

- BUBBLE SORT (also known as ripple sort)
```
- interactive search with students:
- Begin with the first element (student), look at the element just to the right of it.
- If the element to the right should come before the element on the left, then swap them so they are in order.
- Compare the next element in line with the first one (the original student) and repeat the step above until you run out of elements to compare to.
- Then begin the entire process from the second element (student).
- Continue this process until all students have been sorted.

```
- after the first run, you will know one position, after the second run you will know two etc.
- it can have optimizations included, but you are still comparing each item against each other item, which is n * n
- it is an inefficient search with the worst case being n^2, so for n=1024, it could take 1,048,576 steps

- QUICK SORT
```
- interactive quick sort with students:
- pick a 'pivot' element
- partition the array into 3 parts:
-- first part: all elements that are less than the pivot
-- second part: the pivot itself (only one element)
-- third part: all elements that are greater than or equal to the pivot
- then apply this same process to the first part (all elements that are less than the orignal pivot)
- continue until all partitions are sorted
```
- white board another example emphasizing pivot points
- its order is (n(log n))
- it has a time complexity and space complexity

- WHY DO WE CARE?
- with a database of 12, it doesn't matter much.
- with a database like Facebook of 80,000,000 it matters a lot!
- O(n) = 40,000,000 (because it averages to n/2)
- O(log n) = 17

## Resources

### HTML Resources
- [Open Graph protocol](http://ogp.me/)
- [Google Meta tags](https://support.google.com/webmasters/answer/79812?hl=en)
- [HTML Cheat Sheet](http://htmlcheatsheet.com/)
- [UTF-8](https://en.wikipedia.org/wiki/UTF-8)
- [HTML Accessability](http://www.clarissapeterson.com/2012/11/html5-accessibility/)
- [Reasons to use Accessability](https://www.psd2html.com/blog/importance-of-web-accessibility.html)
- [Emmet Cheatsheet](https://docs.emmet.io/cheat-sheet/)
- [the worlds worst website ever](https://www.theworldsworstwebsiteever.com/)
- [camerons world](http://www.cameronsworld.net/)
- [space jam](https://www.warnerbros.com/archive/spacejam/movie/jam.htm)

### BIG O Resources
- [Quicksort](http://me.dt.in.th/page/Quicksort/)
- [Introduction to computer science algorithms, which continues on to different searches](https://www.khanacademy.org/computing/computer-science/algorithms/intro-to-algorithms/v/what-are-algorithms)
- [Big O Cheatsheet](http://bigocheatsheet.com/)
- [Explaing zero-power, only need the first third of the article](https://medium.com/i-math/the-zero-power-rule-explained-449b4bd6934d)
- [Big O Notation: paragraphs 2-4](https://en.wikipedia.org/wiki/Big_O_notation)


## Example html 5
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>
    <header>
        <nav></nav>
    </header>
    <main>
        <section>
            <article>
                <p></p>
                <p>
                <figure></figure>
                </p>
            </article>
        </section>
    </main>
    <aside></aside>
    <footer></footer>
</body>
</html>
```

## Units
- HTML Intro
- HTML Basics
- HTML Formatting
- HTML Structuring
- Math Big O