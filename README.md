elob_layout_css
===============

elob_layout, a Cascading Style Sheet (CSS), facilitates elastic layout of Web pages suitable for line of business Web applications that sometime display forms of "normal/fixed" width and at other times display reports that are very wide horizontally.


Purpose
===============

The purpose of this CSS to impart a layout that is ubiquitous in line of business (LOB) applications. Typically, a LOB application has:

1) Application banner aligned to the top-side of a Web page that usually displays the title of the application as well as currently logged-in user name (B)

2) Navigation commands aligned to the left-side of a Web page (N)

3) The rest of the Web page real estate (the right-side, C) is used to display content based on the navigation commands chosen. 

4) The footer (F) is present at the bottom of the page.

The above regions are depicted below.

<pre>
-------------------------------------------------------
B - Application Banner          user: me@email.com 
-------------------------------------------------------
N - Navigation |   C - Content
               |
               |
               |
               |
               |
               |
               |
-------------------------------------------------------
F - Footer, Copyright
</pre>			   

The height of the application banner (B) and the width of the navigation (N) regions are known at design time and their dimensions can be regarded as "fixed".

However, the content area (C) may be dependent on the data being displayed. For example, the content area may show a Web form (typically less than 800px) or a tabular report that may be quite a bit wider than the size of the entire device screen.

This CSS aims to control the width of the content area (C) based on width of the content being displayed as follows.

1. When the "narrow" content is displayed, the layout shrinks to a minimum width (960px) that is pleasing to the eye.

2. However, when "wide" content, such as a wide tabular report, is displayed, the layout becomes as wide as the report. The horizontal and vertical scroll bars of the Browser can be used to view the entire content.


Demo
===============

1) Create a new empty directory

2) Copy the following files to the new directory

elob_layout.css

example_narrow.html

example_wide.html

3) Open example_narrow.html in a Web browser to see how the Web page looks like when the content is of a smaller width (such as Web forms).

4) Open example_wide.html in a Web browser to see how the Web page looks like when the content is fairly wide (such as tabular reports). Note how the banner widens and the Browser horizontal scroll bar appears at the bottom.

How to use
===============

1) Simply copy elob_layout.css to wherever you typically store your css files

2) Reference elob_layout.css in your HTML pages.

See example_narrow.html and example_wide.html for examples. Both of these example files use the same css, but have content of different widths.

Thank you for trying elob_layout.css!

Sal Razzaq