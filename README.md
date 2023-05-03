Download Link: https://assignmentchef.com/product/solved-cs1331-homework-09-wizards-duel
<br>
<h1>Problem Description</h1>

You’re a muggle programmer at Hogwarts and you are a big fan of the Duelling Club. As a fan, you enjoy betting and predicting the outcome of the duels. Dumbledore asks you to create a duel simulator to predict the winner of a matchup and to bet appropriately! Using some of your own coding “magic”, you decide to create a class hierarchy that represents the wizards around you.

<h1>Solution Description</h1>

For this assignment, create files with the following names:

<ul>

 <li>java</li>

 <li>java</li>

 <li>java</li>

 <li>java</li>

</ul>

Please make sure to use descriptive variables and javadocs as we will be manually grading most of this assignment. You don’t have to make getters and setters for all variables, just where you think is needed!

<strong>You must use all of the best practices that we have learned in class.</strong>

<strong>Wizard Class:</strong>

<em>Description</em>:

<ul>

 <li>A wizard has a name, health, max health, attack power, favorite color, and spell book.</li>

 <li>We can create a wizard if we know their name, favorite color, max health, attack power, and spell book.

  <ul>

   <li>If we don’t know their max health, let it be 25.</li>

   <li>All wizards have a spell book, and the default spell book has only one spell in it:</li>

  </ul></li>

</ul>

∗ Wingardium Leviosa: 0 attack power

<ul>

 <li>Wizards’ health should be at max when they are created!</li>

</ul>

<em>Functionality</em>:

<ul>

 <li>Wizards can cast spells.

  <ul>

   <li>A wizard will randomly choose one spell from their spell book.</li>

  </ul></li>

 <li>When you print a wizard, we get an output:

  <ul>

   <li>“[name] wishes to join the [color] house at Hogwarts! They have [current health] health points and [attack power of wizard] attack power.”</li>

  </ul></li>

 <li>Two wizards should be able to duel each other. Because they are having a Wizard’s duel, this method should be called on the Wizard class, not something an individual wizard does.

  <ul>

   <li>The duel continues until one of the wizards’ health falls to 0.</li>

  </ul></li>

</ul>

∗ Wizards will deal damage to their opponent.

<ul>

 <li>The amount of damage is attack power of wizard + attack power of spell</li>

</ul>

∗ Each round before the attack phase, There is a 20% chance that the wizard with less health will gain 3 health.

<ul>

 <li>Print “[name] drinks an invigoration potion and restores 3 health! [name] now has [health] health.”</li>

 <li>Wizard’s health should not be able to go above max health.</li>

 <li>If the two wizards have equal health, the potion is not drunken.</li>

</ul>

∗ After taking the potion, the wizard with less health should attack first, then the other wizard attacks back.

<ul>

 <li>If a potion is drunk, check wizard health again. The wizard with the least amount of health should always attack first. This means the wizard who takes the potion may be different from the wizard who attacks first.</li>

 <li>If the two wizards have equal health, you can choose the wizard that attacks first.</li>

</ul>

∗ When each wizard attacks,

<ul>

 <li>Print “[name] casts [spell name] and deals [damage] damage. [other name] now has [other wizard health] health.” ∗ Health cannot fall below 0 at any point.</li>

 <li>If a wizard’s health falls to 0, print “[name] falls to the ground. [other name] wins the duel!”</li>

</ul>

∗ After the duel, restore both wizards’ health to their max health.

<ul>

 <li>Wizards can interact with another wizard.

  <ul>

   <li>prints “[name]: Hey [other name], let’s be friends!” <strong>– </strong>Duel will commence between two wizards.</li>

  </ul></li>

 <li>Correctly decides if two wizards are equal based on: name, health, attack power, color, and spell book.</li>

</ul>

<strong>Gryffindor Class:</strong>

<em>Description</em>:

<ul>

 <li>Gryffindors are also wizards, so they should be able to have/do everything a normal wizard can do!</li>

 <li>We can create a Gryffindor wizard if we know their name.</li>

 <li>Gryffindors focus on resilience and therefore have more health.

  <ul>

   <li>Max health is a random number between 25 to 30 (inclusive).</li>

   <li>Base attacking power is a random number between 4 to 6 (inclusive).</li>

  </ul></li>

 <li>Gryffindors love the color scarlet.</li>

 <li>Gryffindors have a special spell book given by Dumbledore and can cast the following spells:

  <ul>

   <li>Expecto Patronum: 3 attack power</li>

   <li>Expelliarmus: 2 attack power</li>

   <li>Ridikkulus: 1 attack power</li>

   <li>Wingardium Leviosa: 0 attack power</li>

  </ul></li>

</ul>

<em>Functionality</em>:

<ul>

 <li>Interacts with another wizard:

  <ul>

   <li>prints “[name]: Hey [other name], let’s be friends!” <strong>– </strong>Duel will commence between two wizards.</li>

  </ul></li>

</ul>

<strong>Slytherin Class:</strong>

<em>Description</em>:

<ul>

 <li>Slytherins are also wizards, so they should be able to have/do everything a normal wizard can do!</li>

 <li>We can create a Slytherin wizard if we know their name.</li>

 <li>Slytherins focus on self preservation and therefore have stronger attacking power. <strong>– </strong>Max health is a random number between 22 to 27 (inclusive).

  <ul>

   <li>Base attacking power is a random number between 5 to 7 (inclusive).</li>

  </ul></li>

 <li>Slytherins love the color green.</li>

 <li>Slytherins have a special spell book with some dark arts and can cast the following spells:

  <ul>

   <li>Expulso: 3 attack power</li>

   <li>Levicorpus: 2 attack power</li>

   <li>Oppugno: 1 attack power</li>

   <li>Flipendo: 1 attack power</li>

   <li>Wingardium Leviosa: 0 attack power</li>

  </ul></li>

</ul>

<em>Functionality</em>:

<ul>

 <li>Interacts with another wizard:

  <ul>

   <li>prints “[name]: Hey [other name], let’s be friends!” <strong>– </strong>Duel will commence between two wizards.</li>

  </ul></li>

</ul>

<strong>Spell Class:</strong>

<em>Description</em>:

<ul>

 <li>Each spell should have a name and a damage associated with it.</li>

 <li>When you print a spell it will output:

  <ul>

   <li>[spell name]: [damage] attack power</li>

  </ul></li>

 <li>Compares two spells’ name and damage and returns a boolean depending on if the spells are the same.</li>

</ul>

<strong>Note: Each method requires proper JavaDocs (see below for more information)</strong>

<strong>Testing your code:</strong>

Feel free to create your own tests in the main method! Here is an example printed output from a duel:

<ul>

 <li>Harry Potter is a Gryffindor with 30 health, 6 attack power.</li>

 <li>Draco Malfoy is a Slytherin with 27 health, 7 attack power.</li>

</ul>

Draco Malfoy casts Expulso and deals 10 damage. Harry Potter now has 20 health.

Harry Potter casts Expelliarmus and deals 8 damage. Draco Malfoy now has 19 health.

Draco Malfoy drinks an invigoration potion and restores 3 health! Draco Malfoy now has 22 health.

Harry Potter casts Expecto Patronum and deals 9 damage. Draco Malfoy now has 13 health.

Draco Malfoy casts Levicorpus and deals 9 damage. Harry Potter now has 11 health.

Harry Potter casts Expecto Patronum and deals 9 damage. Draco Malfoy now has 4 health.

Draco Malfoy casts Oppugno and deals 8 damage. Harry Potter now has 3 health.

Harry Potter casts Ridikkulus and deals 7 damage. Draco Malfoy now has 0 health. Draco Malfoy falls to the ground. Harry Potter wins the duel!

<h1>Rubric</h1>

<ul>

 <li>[45] java

  <ul>

   <li>[5] Correct constructors</li>

  </ul></li>

</ul>

∗ [5] Constructor chaining and default values

<ul>

 <li>[5] Correct method to cast a spell</li>

 <li>[5] Correct output when printing a wizard</li>

 <li>[5] Correct method to interact with wizards</li>

 <li>[5] Correctly checks if two wizards are the same</li>

 <li>[20] Working duel method</li>

</ul>

∗ [5] Duel continues until health falls to 0 at any point

∗ [5] The wizard with less health attacks first. The other wizard attacks next. Turn order may change after a round

∗ [5] Wizard with less health has 20% chance to gain 3 health

∗ [2] Damage calculation is correct and includes the attack power of spells

∗ [3] Wizards restore their health to their original max health after dueling

<ul>

 <li>[20] java

  <ul>

   <li>[10] Correct constructor</li>

  </ul></li>

</ul>

∗ [5] Correct random range for health and attack power

∗ [5] Constructor chaining

<ul>

 <li>[10] Correct method for interaction</li>

</ul>

∗ [5] Duels

∗ [5] Correct output

<ul>

 <li>[20] java

  <ul>

   <li>[10] Correct constructor</li>

  </ul></li>

</ul>

∗ [5] Correct random range for health and attack power

∗ [5] Constructor chaining

<ul>

 <li>[10] Correct method for interaction</li>

</ul>

∗ [5] Duels

∗ [5] Correct output

<ul>

 <li>[15] java

  <ul>

   <li>[5] Correct constructor</li>

   <li>[5] Correctly checks if two spells are the same <strong>– </strong>[5] Correct output when printing a spell</li>

  </ul></li>

</ul>

<strong>Allowed Imports</strong>

<ul>

 <li>You may import java.util.Random.</li>

</ul>

<h1>Javadocs</h1>

For this assignment, you will be commenting your code with Javadocs. Javadocs are a clean and useful way to document your code’s functionality. For more information on what Javadocs are and why they are awesome, the <a href="http://www.oracle.com/technetwork/java/javase/documentation/index-137868.html">online overview</a> for them is extremely detailed and helpful.

You can generate the javadocs for your code using the command below, which will put all the files into a folder called javadoc:

$ javadoc *.java -d javadoc

The relevant tags that you need to include are @author, @version, @param, and @return. Here is an example of a properly Javadoc’d class:

<table width="632">

 <tbody>

  <tr>

   <td width="632"><strong>import </strong>java.util.Scanner;<em>/**</em>*       This class represents a Dog object<em>.</em>*       <strong>@author </strong>George P<em>. </em>Burdell*       <strong>@version </strong><em>1.0</em><em>*/ </em><strong>public class </strong>Dog {<em>/**</em>*       Creates an awesome dog <em>(</em>NOT a dawg<em>!) */</em><strong>public </strong>Dog() { …</td>

  </tr>

  <tr>

   <td width="632">}<em>/**</em>* This method takes in two ints and returns their sum* <strong>@param a </strong>first number* <strong>@param b </strong>second number <em>* </em><strong>@return </strong>sum of a and b<em>*/</em><strong>public </strong>int add(int a, int b) {…}}</td>

  </tr>

 </tbody>

</table>

A more thorough tutorial for Javadocs can be found <a href="https://cs1331.gitlab.io/cs1331-style-guide.html">here</a>. Take note of a few things:

<ol>

 <li>Javadocs are begun with /** and ended with */.</li>

 <li>Every class you write must be Javadoc’d and the @author and @verion tag included. The comments for a class should start with a brief description of the role of the class in your program.</li>

 <li>Every non-private method you write must be Javadoc’d and the @param tag included for every method parameter. The format for an @param tag is @param &lt;name of parameter as written in method header&gt; &lt;description of parameter&gt;. If the method has a non-void return type, include the @return tag which should have a simple description of what the method returns, semantically.</li>

</ol>


