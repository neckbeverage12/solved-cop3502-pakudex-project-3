Download Link: https://assignmentchef.com/product/solved-cop3502-pakudex-project-3
<br>
<h1>Overview</h1>

This project will provide students with practice building and working with object-oriented programming constructs including classes and objects by building classes to represent creatures and a cataloguing system.

<strong> </strong>

<h1>Scenario</h1>

<strong><em>NOTE: This project concept is a work of satire. To state the obvious: we do not advise one to go around imprisoning creatures in small receptacles held in one’s pockets and/or having them fight for sport. </em></strong>




Pouch Creatures – abbreviated “Pakuri” – are the latest craze sweeping elementary schools around the world. Tiny magical creatures small enough to fit into one’s trouser pouches (with enough force applied, ‘natch) have begun appearing all around the world in forests. They come in all shapes colors. When stolen from their parents at a young enough age, they can be kept in small spherical cages (for their own good) easily carried by elementary school children (though they are also popular with adults). This has led to an unofficial catch phrase for the phenomenon – “Gotta steal ‘em all!” – a play on the abbreviation “Pakuri” (which doubles as Japanese slang meaning “to steal”). Young children can then pit their Pakuri against one another in battle for bragging rights or to steal them from one another. (Don’t worry – they heal their wounds quickly!)




Of course, keeping track of all these critters can be a real task, especially when you are trying to steal so many of them at such a young age! You’ve decided to cash in – hey, if you don’t someone else will – on the morally ambiguous phenomenon by developing an indexing system – a <strong><em>Pakudex</em></strong> – for kids and adult participants.

<h1>Requirements</h1>

Students will construct three classes: a driver class with a <strong>main()</strong> entry point (<strong>PakuriProgram</strong>) and two data object classes (<strong><sub>Pakuri</sub></strong> and <strong><sub>Pakudex</sub></strong>). <u>All attributes / methods must be private unless noted in the specification!</u>




<table width="289">

 <tbody>

  <tr>

   <td width="289">Welcome to Pakudex: Tracker Extraordinaire!Enter max capacity of the Pakudex: <strong>30</strong>The Pakudex can hold 30 species of Pakuri. Pakudex Main Menu—————–1.  List Pakuri2.  Show Pakuri3.  Add Pakuri4.  Evolve Pakuri5.  Sort Pakuri6.  ExitWhat would you like to do?</td>

  </tr>

 </tbody>

</table>

<h2>PakuriProgram Class (Driver / Program) <sup> </sup></h2>

When run, the program should…

<ul>

 <li>Display a welcome message</li>

 <li>Prompt for / read Pakudex capacity &amp; confirm</li>

 <li>Display the menu</li>

 <li>Prompt for input</li>

</ul>










<u>Listing Pakuri</u>

This should number and list the critters in the Pakudex in the order contained. For example, if “Pikaju” and “Charasaurus” were added to the Pakudex (in that order), before sorting, the list should be:




<h3>            Success                                                                           Failure</h3>

<table width="677">

 <tbody>

  <tr>

   <td width="339">Pakuri In Pakudex:1.  Pikaju2.  Charasaurus</td>

   <td width="11"></td>

   <td width="328">No Pakuri in Pakudex yet! Pakudex Main Menu</td>

  </tr>

 </tbody>

</table>




<u>Show Pakuri</u>

The program should prompt for a species and collect species information, then display it:




<h3>            Success                                                                           Failure</h3>

<table width="677">

 <tbody>

  <tr>

   <td width="339">Enter the name of the species to display: <strong>PsyGoose</strong> Species: PsyGooseAttack: 65Defense: 57Speed: 61</td>

   <td width="11"></td>

   <td width="328">Enter the name of the species to display: <strong>PsyDuck </strong>Error: No such Pakuri! Pakudex Main Menu—————–1. List Pakuri</td>

  </tr>

 </tbody>

</table>




<u>Adding Pakuri</u>

When adding a Pakuri, a prompt should be displayed to read in the species name, and a confirmation displayed following successful addition (or failure).




<h3>            Success                                                                           Failure – Duplicate</h3>

<table width="339">

 <tbody>

  <tr>

   <td width="339">Enter the name of the species to add: <strong>PsyGoose</strong>Pakuri species PsyGoose successfully added! Pakudex Main Menu—————–</td>

  </tr>

 </tbody>

</table>

<table width="328">

 <tbody>

  <tr>

   <td width="328">Enter the name of the species to add: <strong>PsyGoose</strong> Error: Pakudex already contains this species!</td>

  </tr>

 </tbody>

</table>

<table width="328">

 <tbody>

  <tr>

   <td width="328">Error: Pakudex is full!</td>

  </tr>

 </tbody>

</table>

<em>Failure – Full </em>




<u>Evolve Pakuri</u>

The program should prompt for a species and then cause the species to evolve if it exists:




<h3>            Success                                                                           Failure</h3>

<table width="677">

 <tbody>

  <tr>

   <td width="339">Enter the name of the species to evolve: <strong>PsyGoose</strong> PsyGoose has evolved!</td>

   <td width="11"></td>

   <td width="328">Enter the name of the species to evolve: <strong>PsyDuck</strong> Error: No such Pakuri!</td>

  </tr>

 </tbody>

</table>

<em> </em>

<u>Sort Pakuri</u>

<table width="330">

 <tbody>

  <tr>

   <td width="330">Pakuri have been sorted!</td>

  </tr>

 </tbody>

</table>

Sort Pakuri in Java standard lexicographical order: <sub> </sub><sub> </sub>




<u>Exit</u>

<table width="330">

 <tbody>

  <tr>

   <td width="330">Thanks for using Pakudex! Bye!</td>

  </tr>

 </tbody>

</table>

Quit the program: <sub> </sub>

<strong> </strong>

<h2>Pakuri Class</h2>

This class will be the blueprint for the different critter objects that you will create. You will need to store information about the critter’s species, attack level, defense level, and speed. All variables storing information about the critters <strong>must be private</strong> (in accessible from outside of the class). We recommend (but do not mandate) the following variable types and names:




<strong>String</strong> species;

<strong>int</strong> attack, defense, speed;




These attack, defense, and speed levels should have the following initial values when first created:




<table width="312">

 <tbody>

  <tr>

   <td width="78"><strong>Attribute </strong></td>

   <td width="233"><strong>Value </strong></td>

  </tr>

  <tr>

   <td width="78">attack</td>

   <td width="233">(species.length() * 7) + 9</td>

  </tr>

  <tr>

   <td width="78">defense</td>

   <td width="233">(species.length() * 5) + 17</td>

  </tr>

  <tr>

   <td width="78">speed</td>

   <td width="233">(species.length() * 6) + 13</td>

  </tr>

 </tbody>

</table>




<em>(You may have noticed Pakuri don’t have individual names, just species; don’t worry! They won’t live long enough for it to matter with all of the fighting. Your conscience can be clear!) </em>







<u>The class must also have the following methods and behaviors (<strong>this is mandatory</strong>):</u>




<em>public</em> <strong>Pakuri</strong>(String species)

This method should be the <strong>only</strong> constructor for this class. <u>There should not be a default constructor!</u>




<em>public</em><em> String</em> <strong>getSpecies</strong>()

Returns the species of this critter




<em>public</em><em> int</em> <strong>getAttack</strong>()

Returns the attack value for this critter




<em>public</em><em> int</em> <strong>getDefense</strong>()

Returns the defense value for this critter




<em>public</em><em> int</em> <strong>getSpeed</strong>()

Returns the speed of this critter




<em>public</em><em> void</em> <strong>setAttack</strong>(int newAttack)

Changes the attack value for this critter to <strong>newAttack</strong>

<strong> </strong>

<em>public</em><em> void</em> <strong>evolve</strong>()

Will evolve the critter as follows: a) double the attack; b) quadruple the defense; and c) triple the speed

<strong> </strong>

<strong> </strong>

<u>Optionally, students may implement the </u><strong><u><sub>Comparable</sub></u></strong><u> interface and its methods:</u>




<em>public</em><em> int</em> <strong>compareTo</strong>(Pakuri target)

Returns integer determining order of <strong>this</strong> object and <strong>target</strong> object (see <strong>Comparable</strong> API for details)

<strong> </strong>

<em>We will not test for this method’s proper function; students may implement as desired (if at all) according to design for the rest of the program. </em>




<h2>Pakudex Class</h2>

The <strong><sub>Pakudex</sub></strong> class will contain all the Pakuri that you will encounter as <strong><sub>Pakuri</sub></strong> objects. Note: The Pakudex will have a set size determined by user input at the beginning of the program’s run; the number of species contained in the Pakudex will never grow beyond this point.







<u>The class must also have the following methods and behaviors (<strong>this is mandatory</strong>):</u>




<em>public</em> <strong>Pakudex</strong>()

Default constructor; if called, the default size for the Pakudex should be 20




<em>public</em> <strong>Pakudex</strong>(int capacity)

Initializes this object to contain exactly <strong><sub>capacity</sub></strong> objects when completely full




<em>public</em><em> int</em> <strong>getSize</strong>()

Returns the number of critters currently being stored in the Pakudex

<em> </em><em>public</em><em> int</em> <strong>getCapacity</strong>()

Returns the number of critters that the Pakudex has the capacity to hold at most

<em> </em><em>public</em><em> String[]</em> <strong>getSpeciesArray</strong>()

Returns a <strong><sub>String</sub></strong> array containing the species of the critters as ordered in the Pakudex; if there are no species added yet, this method should return <strong><sub>null</sub></strong>

<strong> </strong>

<em>public</em><em> int[]</em> <strong>getStats</strong>(String species)

Returns an <strong><sub>int</sub></strong> array containing the attack, defense, and speed statistics of <strong><sub>species</sub></strong> at indices 0, 1, and 2 respectively; if <strong>species</strong> is not in the Pakudex, returns <strong>null</strong>

<strong> </strong>

<em>public</em><em> void</em> <strong>sortPakuri</strong>()

Sorts the <strong><sub>Pakuri</sub></strong> objects in this <strong><sub>Pakudex</sub></strong> according to Java standard lexicographical ordering of species name




<em>public</em><em> boolean</em> <strong>addPakuri</strong>(String species)

Adds <strong>species</strong> to the Pakudex; if successful, return <strong>true</strong>, and <strong>false</strong> otherwise

<strong> </strong>

<em>public</em><em> boolean</em> <strong>evolveSpecies</strong>(String species)

Attempts to evolve <strong>species</strong> within the Pakudex; if successful, return <strong>true</strong>, and <strong>false</strong> otherwise

<strong> </strong>