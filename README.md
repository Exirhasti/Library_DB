<h1 align="center">📚 Library Management System (MySQL Project)</h1>

<p align="center">
  A relational database system for managing a university library using <b>MySQL</b>, including students, books, loans, reservations, penalties, and automated triggers.
</p>

<hr>

<h2>📌 Project Overview</h2>

<p>
This project implements a fully normalized library database system. It manages:
</p>

<ul>
  <li>👨‍🎓 Students with academic constraints (GPA, level)</li>
  <li>📖 Books with availability tracking</li>
  <li>🔄 Loans and return system</li>
  <li>⏳ Automatic penalty calculation for late returns</li>
  <li>📌 Book reservation system</li>
  <li>🧾 Activity logging system</li>
</ul>

<hr>

<h2>🧱 Database Schema</h2>

<h3>Core Tables</h3>

<ul>
  <li><b>Students</b> — stores student academic information</li>
  <li><b>Books</b> — manages book inventory and status</li>
  <li><b>Admins</b> — library administrators</li>
  <li><b>Loans</b> — tracks borrowed books</li>
  <li><b>Reservations</b> — handles book reservation requests</li>
  <li><b>Penalties</b> — stores late return fines</li>
  <li><b>Logs</b> — system activity tracking</li>
</ul>

<hr>

<h2>⚙️ Key Features</h2>

<ul>
  <li>🔒 <b>Loan Restriction Logic</b> based on student level and GPA</li>
  <li>📚 Automatic book status update (Available ↔ Loaned)</li>
  <li>⏰ Late return detection with fine calculation</li>
  <li>🧾 Full audit log for reservations and loans</li>
  <li>⚡ Trigger-based automation (no external logic needed)</li>
</ul>

<hr>

<h2>🚀 MySQL Features Used</h2>

<ul>
  <li>Triggers (BEFORE / AFTER INSERT, UPDATE)</li>
  <li>Foreign Keys & Referential Integrity</li>
  <li>ENUM types for controlled values</li>
  <li>Default timestamps and computed fields</li>
  <li>Conditional logic inside triggers</li>
</ul>

<hr>

<h2>🧠 Business Rules</h2>

<ul>
  <li>PhD students → max 7 books</li>
  <li>Masters students → max 5 books</li>
  <li>Undergraduate students → max 4–5 books depending on GPA</li>
  <li>Late return → fine = 1000 × days late</li>
</ul>

<hr>

<h2>🗂️ Project Structure</h2>

<pre>
library_db.sql
├── Table Definitions
├── Triggers
├── Sample Data Inserts
└── Logs & Audit System
</pre>

<hr>

<h2>📊 Sample Entities</h2>

<ul>
  <li>👨‍🎓 10 Students</li>
  <li>📖 10 Books</li>
  <li>🧑‍💼 10 Admins</li>
  <li>🔄 Sample Loans, Reservations, and Penalties</li>
</ul>

<hr>

<h2>🛠️ How to Run</h2>

<ol>
  <li>Open MySQL Workbench or any MySQL client</li>
  <li>Create database: <code>CREATE DATABASE library_db;</code></li>
  <li>Run the provided SQL file</li>
  <li>All tables, triggers, and sample data will be created automatically</li>
</ol>

<hr>

<h2>📌 Author</h2>

<p>
Built as a university database project for learning <b>DBMS concepts, relational design, and MySQL triggers</b>.
</p>

<hr>

<p align="center">
  ⭐ If you like this project, give it a star!
</p>
