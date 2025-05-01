# cis3296_Book_Buddies
<h2>Project Abstract</h2>
<p><i>This project proposes a web application that enables users to create or join a book club, providing a customizable and interactive reading experience. Each club owner can assign different roles to its members, allowing for a structured and engaging community. Through a voting system, members can submit book suggestions and collectively decide on the next read, ensuring that everyone has a voice in the selection process. The platform integrates Discord authentication, streamlining the login process and fostering seamless communication among members. By leveraging scheduled book discussions, users can easily engage in meaningful conversations about their current reads, enhancing the collaborative nature of the book club experience.</i></p>

<h2>Conceptual Design</h2>
<p>All development of this web application will be done on the operating system Ubuntu (which can easily be installed using WSL) and the programming language will be Python using the web framework Django. Since Django supports SQLite natively, that will also be the database that will be used.  The web Application will have the following pages: </p>
<ul>
  <li><strong>Home Page</strong></li>
    <p>The home page will have an option to create an account or login. The main content area of this page will be reasons why the user should use this website.</p>
  <li><strong>Account Page</strong></li>
    <p>The account page will simply display all the user account details such as Book clubs joined or created, books nominated, and books completed reading.</p>
  <li><strong>Log In Page</strong></li>
  <p>This page will display an option to either create an account or Login if they have an existing account already. All accounts will be created using the Discord OAuth2 API. </p>
  <li><strong>Create Club Page</strong></li>
  <p>This page will allow the user to create a new book club via a Django Form that will then create a new record in the database. </p>
  <li><strong> Club Activity Page</strong></li>
  <p>Each club will have an activity page that will list all the members of the club, all books that have been suggested to be read, and books that have been completed by the club. Members that have admin privileges will have extra options available to them such as membership removal and nominated book history editing.</p>
  <li><strong>Voting Page</strong></li>
  <p>This page will display all the books that have been selected by users in the club for the current round of voting. Each Book being suggested will have a short description and other related information to entice users to vote for said book. This information will be obtained via the Google Books API.</p>
</ul>

<h2>How to Run</h2>
<ol>
  <li>Ensure Python3 is installed on development computer</li>
<li>Fork repository</li>
<li>Git clone repository into a Ubuntu operating system folder (can be WSL)</li>
<li>Create a virtual environment using command: </li>
<ol><li>python3 -m venv myenv</li></ol>
<li>Activate the virtual environment with the command:</li>
<ol><li>source myenv/bin/activate</li></ol>
<li>Navigate to the folder called djangotutorial and type the command: </li>
<ol><li>pip install -r requirements.txt</li></ol>
<li>Start local server by typing the command:</li> 
<ol><li>python manage.py runserver</li></ol>
<li>Visit <a href="http://127.0.0.1:8000">http://127.0.0.1:8000</li>

</ol>
