<h1 align="center">Course Registration Planner</h1>

<p align="center">
<strong>A Python-based planner that generates valid semester-by-semester course schedules from prerequisite data.</strong>
<br/>
Uses graph traversal and heap-based prioritization to produce optimized, constraint-aware registration plans.
</p>

---

<h2>About</h2>

This project models course prerequisites as a directed graph and generates a valid registration plan that respects dependency constraints while limiting each semester to a maximum of four courses.

The system detects invalid prerequisite cycles, computes course depth to prioritize scheduling, and outputs an ordered, semester-by-semester plan designed to reflect realistic academic planning.

---

<h2>Goal & Requirements</h2>

<strong>Primary objectives:</strong>
<ul>
  <li>Model course prerequisites using a directed graph</li>
  <li>Detect and reject cyclic prerequisite structures</li>
  <li>Generate a valid topological ordering of courses</li>
  <li>Group courses into semesters with a maximum load of four per term</li>
</ul>

<strong>Constraints:</strong>
<ul>
  <li>Courses must be taken only after all prerequisites are completed</li>
  <li>No more than four courses per semester</li>
  <li>Invalid prerequisite graphs (cycles) must be detected and reported</li>
</ul>

---

<h2>Key Learnings</h2>

<ul>
  <li>Implementing graph traversal using depth-first search (DFS)</li>
  <li>Detecting cycles in directed graphs</li>
  <li>Using computed depth to prioritize scheduling decisions</li>
  <li>Applying binary heaps to manage course ordering efficiently</li>
</ul>

---

<h2>Technologies</h2>

<ul>
  <li>Python</li>
  <li>Directed graphs & DFS</li>
  <li>Topological ordering</li>
  <li>Binary heap (priority queue)</li>
  <li>Unit testing (<code>unittest</code>)</li>
</ul>

---

<h2>Running the Project</h2>

<ol>
  <li>Clone the repository</li>
  <li>Provide course and prerequisite data via standard input</li>
  <li>Run the program:
    <pre><code>python registration.py &lt; input.txt</code></pre>
  </li>
</ol>

The program outputs a validated, semester-by-semester registration plan if one exists.

---

<h2>Project Status</h2>

Completed — fully tested and stable.  
Designed for clarity, correctness, and extensibility.

---

<h2>Context</h2>

Built as part of coursework at <strong>The University of Texas at Austin</strong> to practice graph-based problem solving, algorithm design, and constraint-driven scheduling.

---

<h2>Author</h2>

<strong>Lillian Pecoraro</strong>  
<a href="https://github.com/lilypecoraro" target="_blank">github.com/lilypecoraro</a>
