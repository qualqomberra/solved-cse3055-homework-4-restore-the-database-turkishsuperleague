Download Link: https://assignmentchef.com/product/solved-cse3055-homework-4-restore-the-database-turkishsuperleague
<br>
<strong>Homework #4 </strong>

Consider the <em>Turkish Super League</em> database that has been e-mailed to you.

<strong><em>player</em></strong><em> (<u>playerID</u></em><em>: int</em><em>, firstName</em><em>: nvarchar(25)</em><em>, lastName</em><em>: nvarchar(25)</em><em>, nationality</em><em>: varchar(25)</em><em>, birthDate</em><em>: </em>

<em>smalldatetime</em><em>, age</em><em>: smallint</em><em>, position</em><em>: varchar(25)</em><em>) </em>

<strong><em>team</em></strong><em> (<u>teamID</u></em><em>: int</em><em>, name</em><em>: nvarchar(50)</em><em>, city</em><em>: nvarchar(25)</em><em>) <strong>player_team</strong> (<u>playerID</u></em><em>: int</em><em>, <u>teamID</u></em><em>: int</em><em>, <u>season</u></em><em>: varchar(5)</em><em>) </em>

<strong><em>match</em></strong><em> (<u>matchID</u></em><em>: int</em><em>, homeTeamID</em><em>: int</em><em>, visitingTeamID</em><em>: int</em><em>, dateOfMatch</em><em>: smalldatetime</em><em>, week</em><em>: tinyint</em><em>) <strong>goals</strong> (<u>matchID</u></em><em>: int</em><em>, <u>playerID</u></em><em>: int</em><em>, isOwnGoal</em><em>: bit</em><em>, <u>minute</u></em><em>: tinyint</em><em>) </em>

<u>Notes</u>:

<ul>

 <li>Table <em>match</em> stores data only for season 2013-2014.</li>

 <li>Table <em>goals</em> stores data only for season 2013-2014.</li>

 <li>Restore the database <em>TurkishSuperLeague</em> using the file <em>bak</em> that has been e-mailed to you. Write the following SQL queries, in only one statement, using this database. For each of the following query, take a screenshot of both your SQL query and output of the query on MS SQL Server.</li>

 <li> Update the field <em>age</em> for all players.</li>

 <li>List the “younger” players whose first name does not contain “nec” and play in “Beşiktaş”. “Younger” players are the ones whose ages are less than the average age of all players. Retrieve playerID, firstname + ” “ + lastname.</li>

 <li>Update all <em>city</em> values of the table <em>team</em> as: “city” + “ #p” + “number of players” +” g” + “number of goals forward” (e.g. “İstanbul #p25 g74”). Do not forget to include own goals in your calculations.</li>

 <li> List the top 10 top scorers. Retrieve playerID, first name, last name, number of goals scored, number of matches that player did not score a goal, average number of goals per scored matches.</li>

</ul>