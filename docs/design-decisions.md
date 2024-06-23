---
title: Design Decisions
nav_order: 3
---

{: .label }
[Jane Dane]

{: .no_toc }
# Design decisions

<details open markdown="block">
{: .text-delta }
<summary>Table of contents</summary>
+ ToC
{: toc }
</details>


## 01: [CSS Style]
### Meta

Status
: **Work in progress** 

Updated
: 20.06.2024

### Problem statement

For the web application, we need a CSS file or at least some CSS to style the web application. The problem is that writing custom CSS code for the entire site is very time-consuming, and since we don't have much time, we need to find a quick solution that allows us to style the website according to our preferences.

### Decision

We (Majd) have decided to use Bootstrap as a framework to create the CSS styles for the website for the following reasons. Firstly, using Bootstrap offers a significantly faster development process compared to writing our own CSS file, which is crucial for us as we don't have a lot of time and want to focus on the database and the functionality of the web application. Secondly, Bootstrap includes a built-in responsive grid system that makes it easier to adapt to different screen sizes.

### Regarded options
	
Pro	Con

Custom CSS File	-Full control over the styling
-Unique, custom design	-Time-consuming
Bootstrap	-Fast development
-Low effort
-Suitable for CSS beginners	-High load time due to the many Bootstrap libraries
-Less design flexibility

----

## 02: [Database]
### Meta

Status
: **Work in progress** 

Updated
: 20-06-2024

### Problem statement

Our goal is to set up a database for our web application where we can manage tables with values. We want to be able to upload, add, delete, and create tables and tuples easily, without writing extensive code. Additionally, we need the capability to upload pictures for the bakery's offers.

### Decision

Our decision is to use Google Firebase. We chose this platform because it is fast and easy to use, thanks to its well-defined methods. This simplifies our programming process, eliminating the need for lengthy SQL queries that can often lead to small, hard-to-detect mistakes. Also, we already has some experience with Firebase's Realtime Database and Storage for uploading pictures, which will be beneficial for our project.

### Regarded options

	Pro	Con
Google Firebase	- We know how to write
-  Fast and easy to use, because of well-defined methods.
 	- SQLAlchemy not possible

Plain Sql	- We know how to write 
	- Need for lengthy SQL queries
SQLAlchemy	- No need for lengthy SQL queries	- We must learn ORM concept & SQLAlchemy
---
