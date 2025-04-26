# eecs-281---programming-project-2-solved
**TO GET THIS SOLUTION VISIT:** [EECS 281 – Programming Project 2 Solved](https://www.ankitcodinghub.com/product/eecs-281-programming-project-2-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;76494&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;5&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (5 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;EECS 281 –  Programming Project 2 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (5 votes)    </div>
    </div>
<strong>Mine All Mine (Priority Queues) </strong>

<h1><strong>Overview </strong></h1>
This project is broken into two parts (A and B). Part A is your main()​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ,​ using the STL std::priority_queue&lt;&gt;; part B is you implementing several different versions of a priority queue.​

<h2>Project Goals</h2>
<ul>
<li>Understand and implement several kinds of priority queues.</li>
<li>Be able to independently read, learn about, and implement an unfamiliar data structure.</li>
<li>Be able to develop efficient data structures and algorithms.</li>
<li>Implement an interface that uses templated “generic” code.</li>
<li>Implement an interface that uses inheritance and basic dynamic polymorphism.</li>
<li>Become more proficient at testing and debugging your code.</li>
</ul>
&nbsp;

<h1>Part A: Gold Mining</h1>
<strong>For Part A, you should always use </strong><strong>std::priority_queue&lt;&gt;</strong>​ <strong>, not your templates from Part B.</strong>​&nbsp;&nbsp;&nbsp; <strong> In Part A you probably do not need or want to use pointers; in Part B you will have to (for the Pairing Heap). </strong>

<h1>Overview</h1>
You are an adventurous gold miner.&nbsp; However, in your avarice you’ve ignored several safe-tunneling practices, and a recent earthquake has left you trapped!&nbsp; Luckily, out of paranoia, you always carry ridiculous quantities of dynamite sticks with you.&nbsp; You need to blast your way out and make the most of each dynamite stick by blasting the piles of rubble which take the fewest sticks to destroy.

<h1>Breaking Out of the Mine</h1>
The mine you are trapped in can be represented with a 2-dimensional grid.&nbsp; There are 2 types of tiles:

<ul>
<li>Tiles containing rubble.</li>
</ul>
○&nbsp;&nbsp;&nbsp; Think of cleared tiles as containing 0 rubble.&nbsp; A tile in the mine could contain 0 before you clear it, that means that it never contained rubble.

<ul>
<li>Tiles containing TNT.</li>
</ul>
&nbsp;

You (the miner) start on a specified tile.&nbsp; At every iteration, you will attempt to blast away the “easiest” tile you can “access”, until you escape!

&nbsp;

<h2>Definition of Discovered</h2>
The mine is very dark and you cannot see very far. When standing on a clear tile there are only four tiles that you can discover from your current tile: up, down, left and right (except for edge-of-map conditions). This is true in every case except for the start of the simulation, when you can only discover the starting tile. Adding tiles to the primary priority queue counts as “discovering” them.&nbsp; They can never be discovered (added to the primary PQ) twice.

&nbsp;

<h2>Definition of Investigating</h2>
The priority queue will always tell you what your “next” tile will be.&nbsp; Investigating is taking the “next” tile from the priority queue and making it your “current” location. When you investigate a tile, you must clear it if it contains rubble or TNT.&nbsp; After clearing the tile, you can then discover any of the four tiles visible from your current location, add them to the priority queue, etc.&nbsp; You use the priority queue to remember tiles that you have discovered, but have not yet investigated.

&nbsp;

<h2>Definition of Easiest Tile</h2>
The easiest tile you can reach is defined as follows, in the stated order:

<ol>
<li>Any TNT tile you can reach.</li>
<li>The lowest rubble-value tile you can reach.</li>
</ol>
&nbsp;

<h2>Tie-breaking</h2>
In the event of ties (two TNT tiles or two rubble tiles with the same rubble-value):

<ol>
<li>Investigate the tile with the lower column coordinate first.</li>
<li>If the tiles have the same column coordinate, investigate the tile with the lower row coordinate.</li>
</ol>
&nbsp;

<h2>Clearing Tiles</h2>
When clearing away rubble tiles, the tile turns into a cleared tile.

When clearing away TNT tiles, the following happens:

<ul>
<li>The TNT tile becomes a cleared tile.</li>
<li>All tiles touching the TNT tile are also “cleared”</li>
</ul>
○&nbsp;&nbsp;&nbsp; If a TNT tile is touching another TNT tile, this will cause a chain explosion.

○&nbsp;&nbsp;&nbsp; Diagonals are not considered for TNT explosions.

&nbsp;

<strong>Definition of Escape </strong>

The miner escapes when their current tile has been cleared and is at the edge of the grid.

<h1>Example</h1>
In the following example, you start at position​ [1,2]​ (row 1, column 2).&nbsp; The tiles that the miner has investigated are ​<strong>red</strong>​ and the tiles that the miner has discovered are ​<strong>blue</strong>​. The tile that the miner just cleared is ​<strong><u>red and underlined</u></strong><u>​</u>. Note: all cleared tiles will be 0, because you must clear a tile as part of investigating it. Positive integers signify rubble tiles (0 is a clear tile) and the value -1 signifies a TNT tile.

&nbsp;

<strong>Please note: </strong>​This example mine is for illustrative purposes and is not the same as the input file described in the ​<strong>Full I/O Example</strong>​ section​<strong>.</strong>​ To make things clearer, there are ​<strong>bold </strong>​indices on the edges that refer to row and column number – they are not a part of the actual input file.

&nbsp;

<strong>&nbsp;&nbsp;&nbsp; 0&nbsp;&nbsp; 1&nbsp;&nbsp; 2&nbsp;&nbsp; 3&nbsp;&nbsp; 4 0</strong>​&nbsp; 20&nbsp; 20&nbsp; 20&nbsp; 20&nbsp; 20 <strong>1</strong>​&nbsp; 20 100&nbsp; ​<strong>10</strong>​&nbsp; 20&nbsp; 15 <strong>2 </strong>​ 20&nbsp; 15&nbsp;&nbsp; 5&nbsp;&nbsp; 0&nbsp; 20

<strong>3</strong>​&nbsp; 20&nbsp; 20&nbsp;&nbsp; 0&nbsp; -1 100

<strong>4</strong>​ 100&nbsp; -1&nbsp; -1&nbsp; 20&nbsp; 20

&nbsp;

At the first iteration, the only tile that can be discovered is the starting location, ​[1,2]​. The miner clears this tile and then can discover other tiles.

&nbsp;

<strong>&nbsp;&nbsp;&nbsp; 0&nbsp;&nbsp; 1&nbsp;&nbsp; 2&nbsp;&nbsp; 3&nbsp;&nbsp; 4 0</strong>​&nbsp; 20&nbsp; 20&nbsp; ​<strong>20</strong>​&nbsp; ​20&nbsp; 20 <strong>1</strong>​&nbsp; 20 ​<strong>100&nbsp;&nbsp; </strong>​<strong><u>0</u></strong>​<strong>&nbsp; 20</strong>​&nbsp; 15 <strong>2</strong>​&nbsp; 20&nbsp; 15&nbsp; ​ ​<strong>5</strong>​&nbsp;&nbsp; 0&nbsp; 20 <strong>3</strong>​&nbsp; 20&nbsp; 20&nbsp;&nbsp; 0&nbsp; -1 100

<strong>4</strong>​ 100&nbsp; -1&nbsp; -1&nbsp; 20&nbsp; 20

&nbsp;

Next, the miner will investigate and clear tile ​[2,2]​ because there are no TNT tiles in view and it has the lowest rubble-value.&nbsp; Clearing that tile allows us to discover more tiles!

&nbsp;

<h2>&nbsp;&nbsp;&nbsp; 0&nbsp;&nbsp; 1&nbsp;&nbsp; 2&nbsp;&nbsp; 3&nbsp;&nbsp; 4</h2>
<strong>0</strong>​&nbsp; 20&nbsp; 20&nbsp; ​<strong>20</strong>​&nbsp; 20&nbsp; 20 <strong>1</strong>​&nbsp; 20 ​ ​<strong>100&nbsp; </strong>​<strong>0</strong>​<strong>&nbsp; 20</strong>​&nbsp; 15 <strong>2</strong>​&nbsp; 20&nbsp; ​<strong>15</strong>​&nbsp; ​ ​<strong><u>0</u></strong>​&nbsp;&nbsp; ​<strong>0</strong>​&nbsp; ​20 <strong>3</strong>​&nbsp; 20&nbsp; 20​<strong>&nbsp;&nbsp; 0&nbsp; </strong>​-1 100 <strong>4</strong>​ 100&nbsp; -1&nbsp; -1&nbsp; 20&nbsp; 20

&nbsp;

The tiles [2,1], [2, 3], and [3,2] are now discoverable (but still uninvestigated). The miner then investigates tile ​[3,2]​. Both this tile and tile ​[2,3]​ have an equally low level of difficulty. The tile ​[3,2] is chosen because its lower column value of ​2​ breaks the tie.

&nbsp;

<h2>&nbsp;&nbsp;&nbsp; 0&nbsp;&nbsp; 1&nbsp;&nbsp; 2&nbsp;&nbsp; 3&nbsp;&nbsp; 4</h2>
<strong>0</strong>​&nbsp; 20&nbsp; 20&nbsp; ​<strong>20</strong>​&nbsp; 20&nbsp; 20 <strong>1</strong>​&nbsp; 20 ​ ​<strong>100&nbsp; </strong>​<strong>0</strong>​<strong>&nbsp; 20</strong>​&nbsp; 15 <strong>2</strong>​&nbsp; 20&nbsp; ​<strong>15</strong>​&nbsp; ​ ​<strong>0</strong>​&nbsp;&nbsp; ​<strong>0</strong>​&nbsp; ​20 <strong>3</strong>​&nbsp; 20&nbsp; ​<strong>20&nbsp;&nbsp; </strong>​<strong><u>0</u></strong>​<strong>&nbsp; -1</strong>​ 100 <strong>4</strong>​ 100&nbsp; -1&nbsp; ​<strong>-1</strong>​&nbsp; 20&nbsp; 20

&nbsp;

At this point, there are two TNT tiles which could be investigated next!&nbsp; However, due to the tie-breaking rules, the miner will choose to blow up the TNT at ​[4,2]​ instead of [3​ ,3]​ (this choice is made because it is at the top of the priority queue).&nbsp; Blowing up the TNT tile at ​[4,2]​ clears all the tiles touching it, creating a chain reaction with the TNT tile at ​[4,1]​.&nbsp; After all the TNT explosions have been resolved, the grid looks like the following:

<h2>&nbsp;&nbsp;&nbsp; 0 &nbsp;&nbsp;1&nbsp;&nbsp; 2&nbsp;&nbsp; 3&nbsp;&nbsp; 4</h2>
<strong>0</strong>​&nbsp; 20&nbsp; 20&nbsp; ​<strong>20</strong>​&nbsp; 20&nbsp; 20 <strong>1</strong>​&nbsp; 20 ​ ​<strong>100&nbsp; </strong>​<strong>0</strong>​<strong>&nbsp; 20</strong>​&nbsp; 15 <strong>2</strong>​&nbsp; 20&nbsp; ​<strong>15</strong>​&nbsp; ​ ​<strong>0</strong>​&nbsp;&nbsp; ​<strong>0</strong>​&nbsp; ​20 <strong>3</strong>​&nbsp; 20​<strong>&nbsp; </strong>​ ​<strong>0&nbsp;&nbsp; </strong>​<strong>0</strong>​<strong>&nbsp; -1</strong>​ 100

<strong>4</strong>​&nbsp;&nbsp; ​<strong>0</strong>​&nbsp;&nbsp; ​<strong>0</strong>​&nbsp;&nbsp; ​<strong><u>0</u></strong>​&nbsp; ​<strong> 0</strong>​<strong>&nbsp; </strong>​20

&nbsp;

An explosion makes tiles ​<em>discovered</em>​ but does not ​<em>investigate</em>​ the tile (or discover around it). So, for example, [3, 1] was blown up by TNT and thus discovered.&nbsp; Therefore it is a candidate to be

investigated next, but [3, 0] (adjacent to it) is not. Since the current location is ​[4,2]​, and this tile is now cleared and on the edge of the map, we have escaped!

<h1>TNT Explosions</h1>
As you will see in the ​<strong>Output</strong>​ section, you need to keep track of the order in which tiles are cleared.

When a TNT tile detonates, <strong>all tiles </strong>​&nbsp; that are cleared as a result of the TNT detonation (including chain​&nbsp; reactions) are cleared in order from “easiest” to “hardest” (as defined in <strong>Breaking Out of the Mine</strong>​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ,​ including tie-breaker rules).&nbsp; These tiles should also be discovered.&nbsp; As stated in <strong>Breaking Out of the</strong>​

<strong>Mine</strong>, do ​ <strong>NOT</strong>​ consider diagonals; even TNT only destroys rubble piles up, down, left and right of it.​

&nbsp;

When a TNT detonation occurs, you should use a priority queue to determine detonation order.&nbsp; Push all the detonated tiles into a separate TNT priority queue, and then pop them out in priority order.&nbsp; You need to use some type of priority queue, because TNT blows up other TNT first, followed by smaller piles of rubble, etc.

&nbsp;

Notice that, as you progress through your TNT priority queue, you may blow up a tile that is already waiting in your primary priority queue.&nbsp; If this happens, you have to make sure that the new rubble value of 0 comes out of the primary PQ sooner than the old, non-0 value.&nbsp; Think about how it will be possible for the primary PQ to actually know that a tile has changed! What if there were two entries for the same tile, and you ignore the second one?&nbsp; See the <strong>Full I/O Example</strong>​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for more details.​

<h1>Command Line</h1>
Your program <strong>MineEscape</strong>​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; should take the following case-sensitive command-line options:​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ●&nbsp;&nbsp;&nbsp; -​ h, –help

○&nbsp;&nbsp;&nbsp; Print a description of your executable and exit(0)​ .​

<ul>
<li>-s, –stats N
<ul>
<li>An optional flag that tells the program it should print extra summarization statistics upon termination. This optional flag has a required argument N.&nbsp; Details are covered in the <strong>Output</strong>​</li>
</ul>
</li>
<li>-m, –median
<ul>
<li>An optional flag that tells the program it should print the median difficulty of clearing a rubble tile that the miner has seen. Details are covered in the <strong>Output</strong>​ ​</li>
</ul>
</li>
<li>-v, –verbose
<ul>
<li>An optional flag that tells the program it should print out every rubble value (or TNT) as a tile is being cleared. Details are covered in the <strong>Output</strong>​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ​</li>
</ul>
</li>
</ul>
&nbsp;

Examples of legal command lines:

<ul>
<li>./MineEscape -v &lt; infile.txt</li>
<li>./MineEscape –stats 15 &lt; infile.txt &gt; outfile.txt</li>
</ul>
&nbsp;

<strong>We will not be error checking your command-line handling, but we expect your program to accept any valid combination of input parameters. </strong>

&nbsp;

<h2>Input and Output Redirection</h2>
In order to read an input file, you will use input redirection, just like you did in project 1. If you want to send your output to a file, you can also use output redirection, as seen in one of the command line examples above. The &lt; redirects​ ​the file specified by the next command line argument to be the standard input (​stdin/cin​) for the program. The &gt; redirects the standard output (​stdout/cout​) of the program to be printed to the file specified by the next command line argument.

<h1>Input</h1>
Settings will be given from an input file, ​<strong>‘MINEFILE’</strong>​ (this input file will not necessarily be named <strong>‘MINEFILE’</strong>​). There will be two different types of input: map (M) and pseudo-random (R).&nbsp; Map input is for your personal debugging, but pseudorandom allows easier testing of large grids.

&nbsp;

<h2><u>Map input mode (M)</u></h2>
Input will be formatted as follows:

<ul>
<li>‘​M​’ – A single character indicating that this file is in map format.</li>
<li>‘​Size​’ – Positive integer number that specifies the size of the square grid (20 means a grid with 20 rows and 20 columns).</li>
<li>‘​Start​’ – Coordinate indicating the starting location, row followed by column (two integers).</li>
</ul>
&nbsp;

Map input consists of a map of all the tiles in the mine.&nbsp; Each tile will be separated from other tiles on the same line with whitespace (any number of spaces or tabs). There are 2 types of tiles:

<ul>
<li>Rubble tiles which are signified by an integer between 0 and 999 (0 means the tile is already clear of rubble).</li>
<li>TNT tiles, which are represented by the integer -1.</li>
</ul>
Tiles are indexed as follows:

<ul>
<li>The tile in the top left corner is at location [0,0].</li>
<li>The tile in the bottom right corner is at location [Size-1,Size-1].</li>
</ul>
&nbsp;

Example of M input (starting location is at [1,2], or row 1 column 2, underlined):

&nbsp;

M

Size: 5

Start: 1 2

9&nbsp;&nbsp;&nbsp; 0&nbsp;&nbsp;&nbsp; 9&nbsp;&nbsp;&nbsp; 3&nbsp;&nbsp;&nbsp; 3&nbsp;&nbsp;&nbsp;&nbsp; 6&nbsp;&nbsp;&nbsp; 9&nbsp;&nbsp;&nbsp; <u>6</u><u>​</u>&nbsp;&nbsp;&nbsp; 8&nbsp;&nbsp;&nbsp; 3<u>​ </u>&nbsp;&nbsp;&nbsp;&nbsp; 9&nbsp;&nbsp;&nbsp; 4&nbsp;&nbsp;&nbsp; 1&nbsp;&nbsp;&nbsp; 9&nbsp;&nbsp;&nbsp; 0

2&nbsp;&nbsp;&nbsp; 0&nbsp;&nbsp; -1&nbsp;&nbsp; -1&nbsp;&nbsp;&nbsp; 9

8&nbsp;&nbsp;&nbsp; 3&nbsp;&nbsp;&nbsp; 9&nbsp;&nbsp;&nbsp; 7&nbsp;&nbsp;&nbsp; 5

&nbsp;

<h2><u>Pseudorandom Mode (R)</u></h2>
&nbsp;

Input will be formatted as follows:

<ul>
<li>‘R’​ – character indicating that this file is in pseudorandom format.</li>
<li>‘Size’​ – Number that specifies the size of the square grid (unsigned integer)</li>
<li>‘Start’ – ​Coordinate indicating the starting location (two unsigned integers, row first).</li>
<li>‘Seed’​ – Number used to seed the random number generator (unsigned integer)</li>
<li>‘Max_Rubble’ ​- The max rubble value a tile can have (unsigned integer)</li>
<li>‘TNT’ ​- Chance that a generated tile will be a TNT tile (20 = 1 in 20 chance of a given tile being a TNT tile, 0 = no chance of TNT; also an unsigned integer)</li>
</ul>
&nbsp;

Example of R input:

&nbsp;

R

Size: 5

Start: 1 2

Seed: 0

Max_Rubble: 10

TNT: 5

&nbsp;

<strong>Generating your grid in R mode: </strong>

Included in Canvas with the project spec are the files ​<strong>P2random.h</strong>​ and ​<strong>P2random.cpp</strong>​ that​ ​contain definitions for the following function:

void P2random::PR_init(std::stringstream&amp; ss, unsigned int floor_size,&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; unsigned int seed, unsigned int max_rubble,&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; unsigned int tnt_chance);

The function ​P2random::PR_init(…)​ will set the contents of the stringstream argument (​ss​) so that you can use it just like you would ​cin​ for M input mode.&nbsp; You may find the following (incomplete) C++ code helpful in reducing code duplication.&nbsp; Remember, ​<strong>DO NOT</strong>​ copy/paste from a PDF file, retype the code by hand!

&nbsp;

​stringstream ss;&nbsp;&nbsp;&nbsp;&nbsp; if (mode == “R”) {

// Read some variables from cin

P2random::PR_init(ss, floor_size, seed, max_rubble, tnt_chance);

} // if

&nbsp;

// If map mode is on, read from cin;&nbsp;&nbsp;&nbsp;&nbsp; // otherwise read from the stringstream&nbsp;&nbsp;&nbsp;&nbsp; istream &amp;inputStream = (mode == “M”) ? cin : ss;

&nbsp;

From this point on, read from ​inputStream​; it doesn’t matter whether the mode is M or R!

&nbsp;

<strong>The example R and M input files given above are equivalent. </strong>​ That is, ​<em>both</em>​ should generate the exact same map!

&nbsp;

<h2>Errors you must check for</h2>
You must make sure that the input file describes a valid mine by checking for each of the following:

<ul>
<li>The character on the first line of the file is either a ‘​M​’ or an ‘​R​’</li>
<li>The coordinate specifying the ‘​Start’​ is a valid location given the ‘​Size​’ of the grid</li>
</ul>
&nbsp;

If you detect invalid input at any time during the program, print a helpful message to ​cerr​ and exit(1)​.&nbsp; ​<strong>You do not need to check for input errors not explicitly mentioned here. </strong>

<strong>&nbsp;</strong>

Look in the Part A samples file, ​Error_messages.txt​: if your program performs an ​exit(1)​ and produces one of those error messages for a valid test case, we’ll show you your error output (to help you debug).

<h1>Output</h1>
<h2>Default Output</h2>
After completing the escape, your program should ​<strong>always</strong>​ print a summary line:

&nbsp;

Cleared ​<strong>&lt;NUM&gt;</strong>​ tiles containing ​<strong>&lt;AMOUNT&gt;</strong>​ rubble and escaped.

<strong>&lt;NUM&gt;</strong> &nbsp;&nbsp;&nbsp; the number of tiles cleared.&nbsp; This number ​<strong>does </strong>​include tiles cleared by TNT, but does not include the TNT tile itself.

<strong>&lt;AMOUNT&gt;</strong> the total rubble cleared.&nbsp; This number ​<strong>does </strong>​include rubble cleared by TNT, but clearing (detonating) the TNT tile itself counts as 0 rubble cleared.

&nbsp;

<h2>Verbose Output</h2>
During the program execution, if the ​-v or​&nbsp;&nbsp;&nbsp;&nbsp; ​ –verbose​ switch is present, each time you clear a tile whose rubble amount is greater than 0, you should print:

<strong>&nbsp;</strong>

Cleared: ​<strong>&lt;RUBBLE&gt;</strong>​ at [​<strong>&lt;ROW&gt;</strong>​,​<strong>&lt;COL&gt;</strong>​]

&nbsp;

<strong>&lt;RUBBLE&gt;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>the amount of rubble being cleared

<strong>&lt;ROW&gt; &lt;COL&gt;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>the coordinates of the tile being cleared

&nbsp;

Any TNT tiles blown up should display:

&nbsp;

TNT explosion at ​<strong>[&lt;ROW&gt;,&lt;COL&gt;]</strong>​!

&nbsp;

Any rubble tiles cleared by TNT should add the words “by TNT” to the cleared line; the general format is:

&nbsp;

Cleared by TNT: ​<strong>&lt;RUBBLE&gt;</strong>​ at [​<strong>&lt;ROW&gt;</strong>​,​<strong>&lt;COL&gt;</strong>​]

&nbsp;

The verbose mode output is produced as tiles are cleared, before the summary line.&nbsp; Consider getting verbose mode working early: it involves very little code, and will help you debug if you have any incorrect output.

&nbsp;

<h2>Median Output</h2>
During the program execution, if the ​-m or​ ​ –median​ switch is present, each time you clear a tile, you should print:

<strong>&nbsp;</strong>

Median difficulty of clearing rubble is: ​<strong>&lt;MEDIAN&gt;</strong>

<strong>&lt;MEDIAN&gt;</strong> The median value of rubble cleared so far. This includes rubble tiles cleared

by TNT, but does not include TNT tiles (-1 values should not be included in this calculation).&nbsp; Tiles that start out clear (rubble value 0) are not included here.

<strong>&nbsp;</strong>

Median output must display 2 decimal digits. You can use:

cout &lt;&lt; std::fixed &lt;&lt; std::setprecision(2); at the beginning of your program to guarantee this.

<strong>&nbsp;</strong>

<h2>Stats Output</h2>
After printing the summary line, if the ​-s​ or ​–stats ​option is specified print the following output (where ​<strong>N</strong>​ is the argument given to the -s flag on the command line):

&nbsp;

<ol>
<li>The line, ​“First tiles cleared:”​ (without quotes) followed by the first ​<strong>N</strong>​ tiles cleared in the following format:</li>
</ol>
&nbsp;

<strong>&lt;TILE_TYPE&gt;</strong>​ at [​<strong>&lt;ROW&gt;</strong>​,​<strong>&lt;COL&gt;</strong>​]

&nbsp;

<strong>&lt;TILE_TYPE&gt;</strong>&nbsp; the type of the tile being cleared.&nbsp; If it is a rubble&nbsp; tile, this is the

rubble amount.&nbsp; If this is a TNT tile, print ​“TNT”​ without the quotes

<strong>&lt;ROW&gt;,&lt;COL&gt; </strong>the coordinates of the tile being cleared.

&nbsp;

<strong>Remember</strong>​: when a TNT tile detonates or when there is a chain reaction, all the tiles are cleared from easiest to hardest.&nbsp; Refer back to ​<strong>TNT Explosions</strong>​ for more details.

&nbsp;

<ol>
<li>The line, ​“Last tiles cleared:”​ (without quotes) followed by the last ​<strong>N</strong> tiles cleared in the​ same format as part ​<strong>A</strong>​.&nbsp; The ​<strong>last</strong>​ tile cleared should be printed first, followed by the second last, etc.</li>
</ol>
&nbsp;

<ol>
<li>The line, ​“Easiest tiles cleared:”​ (without quotes) followed by the ​<strong>N</strong>​ easiest tiles you blew up in the same format as part ​<strong>A </strong>​in ​<em>descending order </em>​(easiest tile followed by next easiest tile)</li>
</ol>
&nbsp;

<ol>
<li>The line, ​“Hardest tiles cleared:”​ (without quotes)’ followed by the​<strong> N</strong>​ hardest tiles you blew up in the same format as part ​<strong>A</strong>. in ​ ​<em>ascending order</em>​ (hardest tile followed by next hardest tile)</li>
</ol>
&nbsp;

If you have cleared less than N tiles, then simply print as many as you can.&nbsp; Tiles that start out clear (rubble value 0) are not included here.

<h1>Full I/O Example</h1>
Input (spec-M.txt​ and ​ spec-R.txt​ ):​

Equivalent input files (the R input file will generate a grid that looks just like the M input file):

M &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; R

Size: 5 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Size: 5

Start: 1 2 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Start: 1 2

9&nbsp;&nbsp;&nbsp; 0&nbsp;&nbsp;&nbsp; 9&nbsp;&nbsp;&nbsp; 3&nbsp;&nbsp;&nbsp; 3 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Seed: 0

6&nbsp;&nbsp;&nbsp; 9&nbsp;&nbsp;&nbsp; 6&nbsp;&nbsp;&nbsp; 8&nbsp;&nbsp;&nbsp; 3 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Max_Rubble: 10

9&nbsp;&nbsp;&nbsp; 4&nbsp;&nbsp;&nbsp; 1&nbsp;&nbsp;&nbsp; 9&nbsp;&nbsp;&nbsp; 0 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; TNT: 5

2&nbsp;&nbsp;&nbsp; 0&nbsp;&nbsp; -1&nbsp;&nbsp; -1&nbsp;&nbsp;&nbsp; 9

8&nbsp;&nbsp;&nbsp; 3&nbsp;&nbsp;&nbsp; 9&nbsp;&nbsp;&nbsp; 7&nbsp;&nbsp;&nbsp; 5

Output:

We ran the program with this command line:&nbsp; <strong>./MineEscape -v -m -s 10 &lt; spec-M.txt</strong>​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; The output is shown below, with the verbose mode​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; highlighted in blue.&nbsp; The median mode output is​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; easy to identify, and statistics come after the “Cleared 6 tiles” summary line. <strong>&nbsp;</strong>

Cleared: 6 at [1,2]

Median difficulty of clearing rubble is: 6.00 Cleared: 1 at [2,2]

Median difficulty of clearing rubble is: 3.50

TNT explosion at [3,2]!

TNT explosion at [3,3]!

Cleared by TNT: 7 at [4,3]

Median difficulty of clearing rubble is: 6.00 Cleared by TNT: 9 at [4,2]

Median difficulty of clearing rubble is: 6.50

Cleared by TNT: 9 at [2,3]

Median difficulty of clearing rubble is: 7.00 Cleared by TNT: 9 at [3,4]

Median difficulty of clearing rubble is: 8.00 Cleared 6 tiles containing 41 rubble and escaped.

First tiles cleared:

6 at [1,2]

1 at [2,2]

TNT at [3,2]

TNT at [3,3]

7 at [4,3]

9 at [4,2]

9 at [2,3]

9 at [3,4] Last tiles cleared:

9 at [3,4]

9 at [2,3]

9 at [4,2]

7 at [4,3]

TNT at [3,3]

TNT at [3,2]

1 at [2,2]

6 at [1,2]

Easiest tiles cleared:

TNT at [3,2]

TNT at [3,3]

1 at [2,2]

<ul>
<li>at [1,2]</li>
<li>at [4,3]</li>
</ul>
9 at [4,2]

9 at [2,3]

9 at [3,4]

Hardest tiles cleared:

9 at [3,4]

9 at [2,3]

9 at [4,2]

7 at [4,3]

6 at [1,2]

1 at [2,2]

TNT at [3,3]

TNT at [3,2]

&nbsp;

<h1>PART B: Priority Queue Implementation</h1>
For this project, you are required to implement and use your own priority queue containers.&nbsp; You will implement a​<strong> “sorted array priority queue”</strong>​, a ​<strong>“binary heap priority queue”</strong>​, and a ​<strong>“pairing heap priority queue”</strong>​ which implement the interface defined in ​<strong>Eecs281PQ.h</strong>​.<strong>&nbsp; </strong>

&nbsp;

To implement these priority queues, you will need to fill in separate header files, ​<strong>SortedPQ.h</strong>​,

<strong>BinaryPQ.h</strong>​, and ​<strong>PairingPQ.h</strong>​, containing all the definitions for the functions declared in

<strong>Eecs281PQ.h</strong>​.&nbsp; We have provided these files with empty function definitions for you to fill in. You may also add any additional functions needed to maintain the priority queue.

&nbsp;

We provide a very bad priority queue implementation called the “​<strong>Unordered priority queue</strong>​” in

<strong>UnorderedPQ.h</strong>​, which does a linear search for the most extreme element each time it is requested. You can look at the code in this priority queue to see the use of ​this-&gt;compare()​ (more on that below), how to write your constructors, etc.&nbsp; There’s also an ​<strong>UnorderedFastPQ.h</strong>​ that is faster; look at how it uses ​mutable​ to accomplish that.. You can also use this priority queue to ensure that your other priority queues are returning elements in the correct order.&nbsp; All priority queues should return elements in the same (priority) order no matter which implementation is being used.

&nbsp;

These files specify more information about each priority queue type, including runtime requirements for each member function and a general description of the container.

&nbsp;

You are not allowed to modify ​<strong>Eecs281PQ.h</strong>​ in any way.&nbsp; Nor are you allowed to change the interface (names, parameters, return types) that we give you in any of the provided headers.&nbsp; You are allowed to add your own private helper functions and variables to the other header files as needed, so long as you still follow the requirements outlined in both the spec and the comments in the provided files.

&nbsp;

These priority queues can take in an optional comparison functor type, ​COMP_FUNCTOR​. Inside the classes, you can access an instance of ​COMP_FUNCTOR​ with ​this-&gt;compare()​. All of your priority queues must default to be MAX priority queues.&nbsp; This means that if you use the default comparison functor with an integer PQ, ​std::less&lt;int&gt;​, the PQ will return the ​<em>largest</em>​ integer when you call top()​. Here, the definition of max (aka most extreme) is entirely dependent on the comparison functor.

For example, if you use ​std::greater&lt;int&gt;​, it will become a min-PQ. The definition is as follows:

&nbsp;

If A is an arbitrary element in the priority queue, and ​top()​ returns the “most extreme” element. this-&gt;compare(top(), A)​ should always return false (A is “less extreme” than ​top()​).

&nbsp;

It might seem counterintuitive that ​std::less&lt;&gt;​ yields a max-PQ, but this is consistent with the way that the STL ​std::priority_queue&lt;&gt;​ works (and other STL functions that take custom comparators, like ​sort()​).

&nbsp;

We will compile your priority queue implementations with our own code to ensure that you have correctly and fully implemented them. To ensure that this is possible (and that you do not lose credit for these tests), do not define a main function in one of the PQ headers, or any header file for that matter.

<strong>Eecs281PQ&lt;&gt;</strong><strong> interface</strong>​

Functions:

push(const TYPE&amp; val) //inserts a new element into the priority //queue

top() &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //returns the highest priority element in the

//priority_queue

pop() &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //removes the highest priority element from

//the priority queue

size() &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //returns the size of the priority queue

empty() &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //returns true if the priority queue is

//empty, false otherwise

&nbsp;

<h2>Unordered Priority Queue</h2>
The ​<em>unordered priority queue</em>​ implements the priority queue interface by maintaining a vector.&nbsp; This has already been implemented for you, and you can use the code to help you understand how to use the comparison functor, etc.&nbsp; Complexities and details are in ​<strong>UnorderedPQ.h</strong>​ and <strong>UnorderedFastPQ.h</strong>​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ​.

<h2>Sorted Priority Queue</h2>
The ​<em>sorted priority queue</em>​ implements the priority queue interface by maintaining a ​<strong>sorted </strong>​vector. Complexities and details are in ​<strong>SortedPQ.h</strong>​.&nbsp; This should be written almost entirely using the STL.&nbsp; The number of lines of code needed to get this working is fairly low, generally &lt;= 10.

<h2>Binary Heap Priority Queue</h2>
Binary heaps will be covered in lecture.&nbsp; We also highly recommend reviewing Chapter 6 of the CLRS book. Complexities and details are in ​<strong>BinaryPQ.h</strong>​. &nbsp;One issue that you may encounter is that the examples and code in the slides use 1-based indexing, but your code must store the values in a vector (where indexing starts at 0).&nbsp; There are three possible solutions to this problem:

&nbsp;

<ul>
<li>Add a “dummy” element at index 0, make sure you never let them access it, and make sure that size()​ and ​empty()​ work properly.</li>
<li>Translate the code from 1-based to 0-based. This is the best solution but the hardest.</li>
<li>Use a function to translate indices for you. Instead of accessing ​data[i]​, use getElement(i)​.&nbsp; The code for ​getElement()​ is given below (both versions are needed).</li>
</ul>
&nbsp;

// Translate 1-based indexing into a 0-based vector​ &nbsp;&nbsp;&nbsp;&nbsp; TYPE &amp;getElement(std::size_t i) {&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return data[i – 1];

} // getElement()

const TYPE &amp;getElement(std::size_t i) const {&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return data[i – 1];

} // getElement()

&nbsp;

<h2>Pairing Priority Queue</h2>
Pairing heaps are an advanced heap data structure that can be quite fast. In order to implement the pairing priority queue, read the two papers we provide you describing the data structure. Complexity details can be found in <strong>PairingPQ.h</strong>​ . We have also included a couple of diagrams that may help you​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; understand the tree structure of the pairing heap.

&nbsp;

Below is the pairing heap modeled as a tree, in which each node is greater than each of its children:

&nbsp;

To implement this structure, the pairing heap will use child and sibling pointers to have a structure like this:

&nbsp;

<h2>Implementing the Priority Queues</h2>
Look through the included header files: you need to add code in ​<strong>SortedPQ.h</strong>​, ​<strong>BinaryPQ.h</strong>​, and

<strong>PairingPQ.h</strong>​, and this is the order that we would suggest implementing the different priority queues. Each of these files has TODO comments where you need to make changes.&nbsp; We wanted to provide you with files that would compile when you receive them, so some of the changes involve deleting and/or changing lines that were only placed there to make sure that they compile.&nbsp; For example, if a function was supposed to return an integer, NOT having a return statement that returns an integer would produce a compiler error.&nbsp; Also, functions which accept parameters have had the name of the parameter commented out (otherwise you would get an unused parameter error).&nbsp; Look at <strong>UnorderedPQ.h</strong>​ as an example, it’s already done.

When you implement each priority queue, you cannot compare ​<em>data</em>​ yourself using the ​&lt;​ operator.&nbsp; You can still use ​&lt;​ for comparisons such as a vector index to the size of the vector, but you must use the provided comparator for comparing the data stored inside your priority queue.&nbsp; Notice that

<strong>Eecs281PQ.h</strong>​ contains a member variable named ​compare​ of type ​COMP​ (one of the templated class types).&nbsp; Although the other classes inherit from ​<strong>Eecs281PQ.h</strong>​, you cannot access the ​compare​ member directly, you must always say ​this-&gt;compare()​ (this is due to a template inheriting from a template).

Notice that in ​UnorderedPQ&lt;&gt;​ it uses ​this-&gt;compare()​ by passing it to the ​max_element() algorithm to use for comparisons.

When you write the ​SortedPQ&lt;&gt;​ you cannot use ​binary_search()​ from the STL, but you wouldn’t want to: it only returns a ​bool​ to tell you if something is already in the container or not!&nbsp; Instead use the lower_bound()​ algorithm (which returns an iterator), and you can also use the ​sort()​ algorithm — you don’t have to write your own sorting function.&nbsp; You do however have to pass the ​this-&gt;compare functor to both ​lower_bound()​ and ​sort()​.

The ​BinaryPQ&lt;&gt;​ is harder to write, and requires a more detailed and careful use of the comparison functor, and you have to know how one works to write one in the first place, even for ​UnorderedPQ&lt;&gt; to use. See the ​<strong>About Comparators</strong>​ section below.

<h2>Compiling and Testing Priority Queues</h2>
You are provided with a testing file, ​<strong>testPQ.cpp</strong>​. ​<strong>testPQ.cpp</strong>​ contains examples of unit tests you can run on your priority queues to ensure that they are correct; however, it is ​<strong>not</strong>​ a complete test of your priority queues; for example it does not test ​updatePriorities()​. It is especially lacking in testing the ​PairingPQ&lt;&gt;​ class, since it does not have any calls to ​addNode()​ or ​updateElt()​. You should add more tests to this source code file.

Using the 281 ​<strong>Makefile</strong>​, you can compile ​<strong>testPQ.cpp</strong>​ by typing in the terminal: ​make testPQ​. You may use your own ​<strong>Makefile</strong>​, but you will have to make sure it does not try to compile your driver program as well as the test program (i.e., use at your own risk).

&nbsp;

<h1>Logistics</h1>
The std::priority_queue&lt;&gt;​

The STL ​std::priority_queue&lt;&gt;​ data structure is basically an efficient implementation of the binary heap which you are also coding in ​<strong>BinaryPQ.h</strong>​. To declare a ​std::priority_queue&lt;&gt;​ you need to state either one or three types:

<ul>
<li>The data type to be stored in the container. If this type has a natural sort order that meets your needs, this is the only type required.</li>
<li>The underlying container to use, usually just a ​std::vector&lt;&gt;​ of the first type. 3) The comparator to use to define what is considered the highest priority element.</li>
</ul>
If the type that you store in the container has a natural sort order (i.e. it supports ​operator&lt;()​), the std::priority_queue&lt;&gt;​ will be a max-heap of the declared type. For example, if you just want to store integers, and have the largest integer be the highest priority:

std::priority_queue&lt;int&gt; pqMax;

When you declare this, by default the underlying storage type is ​vector&lt;int&gt;​ and the default comparator is ​less&lt;int&gt;​. &nbsp;If you want the smallest integer to be the highest priority:

std::priority_queue&lt;int, vector&lt;int&gt;, greater&lt;int&gt;&gt; pqMin;

If you want to store something other than integers, define a custom comparator as described below.

<h2>About Comparators</h2>
The functor must accept two of whatever is stored in your priority queue: if your PQ stores integers, the functor would accept two integers.&nbsp; If your PQ stores pointers to units, your functor would accept two pointers to orders (actually two ​const​ pointers, since you don’t have to modify units to compare them).

Your functor receives two parameters, let’s call them ​a​ and ​b​.&nbsp; It must always answer the following question: ​<strong>is the priority of </strong>​<strong>a</strong>​<strong> less than the priority of </strong><strong>b</strong>​ ​?&nbsp; What does lower priority mean?&nbsp; It depends on your application.&nbsp; For example, refer back to the ​<strong>Breaking Out of the Mine</strong>​ section: if you have multiple tiles in your priority queue, you determine priority based on smallest rubble value.&nbsp; If rubble value is the same, break ties based on column or row number.

When you would have wanted to write a comparison, such as:

if (data[i] &lt; data[j])

You would instead write:

if (this-&gt;compare(data[i], data[j])

Your priority queues must work ​<strong>in general</strong>​. In general, a priority queue has no idea what kind of data is inside of it.&nbsp; That’s why it uses ​this-&gt;compare()​ instead of ​&lt;​.&nbsp; What if you wanted to perform the comparison ​if (data[i] &gt; data[j])​?&nbsp; Use the following:

​if (this-&gt;compare(data[j], data[i])

<h1>Libraries and Restrictions</h1>
For part A, we encourage the use of the STL, with the exception of these prohibited features:

<ul>
<li>The thread/atomics libraries (e.g., boost, pthreads, etc) which spoil runtime measurements.</li>
<li>Smart pointers (both unique and shared).</li>
</ul>
&nbsp;

You ​<strong>are</strong>​ allowed to use ​std::vector&lt;&gt;​, ​std::priority_queue&lt;&gt;​ and std::deque&lt;&gt;​&nbsp;&nbsp;&nbsp; ​.

&nbsp;

You are ​<strong>not</strong>​ allowed to use other STL containers. Specifically, this means that use of ​std::stack&lt;&gt;​, std::queue&lt;&gt;​, ​std::list&lt;&gt;​, ​std::set&lt;&gt;​, ​std::map&lt;&gt;​, ​std::unordered_set&lt;&gt;​, std::unordered_map&lt;&gt;​, and the ​‘multi’​ variants of the aforementioned containers are forbidden.

&nbsp;

For part B,

&nbsp;

You ​<strong>are</strong>​ allowed to use ​std::sort()​.

You ​<strong>are</strong>​ allowed to use ​std::lower_bound()​.

&nbsp;

You are ​<strong>not</strong>​ allowed to use ​std::partition()​, ​std::partition_copy()​, std::partial_sort()​, ​std::stable_partition()​, ​std::make_heap()​, std::push_heap()​, ​std::pop_heap()​, ​std::sort_heap()​, ​std::qsort()​, or anything that trivializes the implementation of the binary heap.

&nbsp;

You are ​<strong>not</strong>​ allowed to use the C++14 regular expressions library (it is not fully implemented on gcc

6.2) or the thread/atomics libraries (it spoils runtime measurements).

&nbsp;

You are ​<strong>not</strong>​ allowed to use other libraries (eg: boost, pthread, etc).

&nbsp;

Furthermore, you may ​<strong>not</strong>​ use any STL component that trivializes the implementation of your priority queues (if you are not sure about a specific function, ask us).

&nbsp;

Your main program (part A) ​<strong>must</strong>​ use ​std::priority_queue&lt;&gt;​, but your PQ implementations (part B) ​<strong>must not</strong>​.

<h1>Testing and Debugging</h1>
Part of this project is to prepare several test files that will expose defects in the program.&nbsp; ​<strong>We strongly recommend</strong>​ that you ​<strong>first</strong>​ try to catch a few of our buggy solutions with your own test files, before beginning your solutions.&nbsp; This will be extremely helpful for debugging.&nbsp; The autograder will also tell you if one of your own test files exposes bugs in your solution.

&nbsp;

<h2>Test File Details</h2>
<strong>Your test files must be valid Map mode input files.</strong>​ We will run your test files on several buggy project solutions.&nbsp; If your test file causes a correct program and the incorrect program to produce different output, the test file is said to expose that bug.

&nbsp;

Test files should be named ​<strong>test-n-&lt;FLAGS&gt;.txt</strong>​ where 0 &lt; ​<em>n</em>​ &lt;= 10.&nbsp; The &lt;FLAGS&gt; portion of the name should contain at least one of ​’m’​ (median), ​’s’​ (statistics), and/or ​’v’​ (verbose).&nbsp; You must specify at least one flag; you can specify two or three if you want.&nbsp; If the ‘s’ flag is specified, the autograder will pick the number of statistics based on the test number (a larger value of ​<em>n</em>​ will generate more statistics).&nbsp; For example, ​<strong>test-1-vs.txt</strong>​ is a valid file name.

&nbsp;

Your test files must be in map input mode and cannot have a size larger than 15.&nbsp; You may submit up to 10 test files (though it is possible to get full credit with fewer test files).&nbsp; The tests the autograder runs on your solution are NOT limited to having a ​Size​ of 15; your solution should not impose any size limits (as long as sufficient system memory is available).&nbsp; However you can assume that an ​int​ (signed or unsigned) can hold the size, row or column number, amount of rubble, etc.

<h1>Submitting to the Autograder</h1>
Do all of your work (with all needed files, as well as test files) in some directory other than your home directory. This will be your “submit directory”. You can make two separate projects inside of your IDE: one for part A, another for part B.&nbsp; Before you turn in your code, be sure that:

<ul>
<li>Every source code and header file contains the following project identifier in a comment at the top of the file: // Project Identifier: 19034C8F3B1196BF8E0C6E1C0F973D2FD550B88F​ The Makefile must also have this identifier (in the first TODO block).</li>
<li>DO NOT copy the above identifier from the PDF! It might contain hidden characters. Copy it from the README file instead (this file is included on Canvas).</li>
<li>You have deleted all .o files and any executables. Typing ‘make clean​ ’ should​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; accomplish this.</li>
<li>Your makefile is called Makefile. Typing ‘make -R -r​ ’ builds your code without errors​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; and generates an executable file called MineEscape​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; . The command line options ​&nbsp;&nbsp; -​ R and ​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; -​ r disable automatic build rules, which will not work on the autograder.</li>
<li>Your Makefile specifies that you are compiling with the gcc optimization option -​ O3. This​ is extremely important for getting all of the performance points, as -​ O3 can often speed up​ execution by an order of magnitude. You should also ensure that you are not submitting a Makefile to the autograder that compiles with -​ g, as this will slow your code down considerably.​ If your code “works” when you don’t compile with -​ O3 and breaks when you do, it means you​ have a bug in your code!</li>
<li>Your test files are named test-n-MODE.txt​ and no other project file names begin​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; with test. Up to 10 test files may be submitted.</li>
<li>The total size of your solution and test files does not exceed 2MB.</li>
<li>You don’t have any unnecessary files (including temporary files created by your text editor and compiler, etc) or subdirectories in your submit directory (i.e. the .git folder used by git source code management).</li>
<li>Your code compiles and runs correctly using version 6.2.0 of the g++ compiler. This is available on the CAEN Linux systems (that you can access via login.engin.umich.edu). Even if everything seems to work on another operating system or with different versions of GCC, the course staff will not support anything other than GCC 6.2.0 running on Linux (students using other compilers and OS did observe incompatibilities). <strong>In order to compile with g++ version</strong>​ <strong>2.0 on CAEN you must put the following at the top of your Makefile (or use the one that we’ve provided): </strong></li>
</ul>
PATH := /usr/um/gcc-6.2.0/bin:$(PATH)

LD_LIBRARY_PATH := /usr/um/gcc-6.2.0/lib64

LD_RUN_PATH := /usr/um/gcc-6.2.0/lib64

Turn in all of the following files:

<ul>
<li>All your .h and .cpp files for the project (solution and priority queues)</li>
<li>Your Makefile ● Your test files</li>
</ul>
You must prepare a compressed tar archive (.tar.gz file) of all of your files to submit to the autograder. One way to do this is to have all of your files for submission (and nothing else) in one directory. Go into this directory and run one of these two commands (assuming you are using our Makefile):

make fullsubmit (​ builds a “tarball” named fullsubmit.tar.gz​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; that contains all source​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; and header files, test files, and the Makefile​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ; this file is to be submitted to the autograder for​ any completely graded submission)

make partialsubmit (​ builds a “tarball” named partialsubmit.tar.gz​&nbsp;&nbsp;&nbsp;&nbsp; that contains​&nbsp;&nbsp; only source and header files, and the Makefile​ ; test files are not included, which will speed up​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; the autograder by not checking for bugs; this should be used when testing the simulation only)

For Part A, you can submit test files (map files), for Part B you only submit code.

&nbsp;

These commands will prepare a suitable file in your working directory. Submit your project files directly to either of the two autograders at: <a href="https://g281-1.eecs.umich.edu/">https://g281-1.eecs.umich.edu/</a> or<u>​ </u> ​ <a href="https://g281-2.eecs.umich.edu/">h</a><u>​ </u><a href="https://g281-2.eecs.umich.edu/">ttps://g281-2.eecs.umich.edu/</a>.<u>​</u>

<h2>You can safely ignore and override any warnings about an invalid security certificate. When the​&nbsp; autograders are turned on and accepting submissions, there will be an announcement on</h2>
<strong>Piazza.</strong> The autograders are identical and your daily submission limit will be shared (and kept track of)​&nbsp;&nbsp; between them. You may submit up to 2 times per calendar day, per part, with autograder feedback (more in Spring). For this purpose, days begin and end at midnight (Ann Arbor local time). We will use your best submission when running final grading. Part of programming is knowing when you are done (when you have achieved your task and have no bugs); this is reflected in this grading policy. We strongly recommend that you use some form of revision control (ie: SVN, GIT, etc) and that you ‘commit’ your files every time you upload to the autograder so that you can always retrieve an older version of the code as needed. Please refer to your discussion slides and Canvas regarding the use of version control.

If you use late days on this project, it is applied to both parts.&nbsp; So if you use one late day for Part A, you automatically get a 1-day extension for Part B, but are only charged for the use of one late day.

<strong>Please make sure that you read all messages shown at the top section of your autograder results! These messages will help explain some of the issues you are having (such as losing points for having a bad Makefile).&nbsp; Also be sure to check whether the autograder shows that one of your own test files exposes a bug in your solution (at the bottom of the student test files section).&nbsp; Watch for the word “Hint” in the autograder feedback about specific test cases.</strong>

<h1>Grading</h1>
<ul>
<li>60 pts total for part A</li>
</ul>
○&nbsp;&nbsp;&nbsp; 45 pts — correctness &amp; performance

○&nbsp;&nbsp;&nbsp; 5 pts — memory leaks

○&nbsp;&nbsp;&nbsp; 10 pts — student-provided test files ●&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 40 pts total for part B

○&nbsp;&nbsp;&nbsp; 20 pts — pairing heap correctness &amp; performance

○&nbsp;&nbsp;&nbsp; 5 pts — pairing heap memory leaks

○&nbsp;&nbsp;&nbsp; 10 pts — binary heap correctness &amp; performance

○&nbsp;&nbsp;&nbsp; 5 pts — sorted heap correctness &amp; performance

&nbsp;

<strong>We also reserve the right to deduct up to 5 points for bad programming style, code that is unnecessarily duplicated, etc.. </strong>

&nbsp;

Refer to the Project 1 spec for details about what constitutes good/bad style, and remember:

&nbsp;

It is <strong>extremely helpful</strong>​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; to compile your code with the gcc options (default in our ​&nbsp;&nbsp;&nbsp;&nbsp; <strong>Makefile</strong>​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ):​ -​ Wall -Werror -Wextra -Wvla -pedantic.&nbsp; This will help you catch bugs in your code early by having the​ compiler point out when you write code that is either of poor style or might result in unintended behavior.

<h1>Appendix A: Printing out the Grid</h1>
While this is never required for the project assignment, you may find it helpful to be able to print out the state of the grid in a human readable format.&nbsp; Unfortunately, the values of rubble may have a different number of digits, which can make it hard to read.&nbsp; For example, consider the following grid:

&nbsp;

10 5 100

200 400 200

1 1 -1

&nbsp;

It is fairly hard to see which tiles touch which other tiles because they do not line up well.&nbsp; Luckily, the header &lt;​ iomanip&gt; contains the definition for the ​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; std::setw()​&nbsp;&nbsp; stream manipulator.​

&nbsp;

The following code snippet gives a quick example of how to use it:

&nbsp;

#include &lt;iomanip&gt;

#include &lt;iostream&gt;

#include &lt;vector&gt;

&nbsp;

using namespace std;

int main() {&nbsp;&nbsp; vector&lt;int&gt; ints1 = {0, 24, 100, 5}; &nbsp;&nbsp;vector&lt;int&gt; ints2 = {100, 2, 40, 2};&nbsp;&nbsp; for(auto i : ints1)&nbsp;&nbsp;&nbsp;&nbsp; cout &lt;&lt; setw(4) &lt;&lt; i;&nbsp;&nbsp; cout &lt;&lt; endl;&nbsp;&nbsp; for(auto i : ints2)&nbsp;&nbsp;&nbsp;&nbsp; cout &lt;&lt; setw(4) &lt;&lt; i;&nbsp;&nbsp; cout &lt;&lt; endl;&nbsp;&nbsp; return 0;

} // main()

&nbsp;

<strong>Output: </strong>

0&nbsp; 24 100&nbsp;&nbsp; 5

100&nbsp;&nbsp; 2&nbsp; 40&nbsp;&nbsp; 2

&nbsp;

In the previous project, using iomanip​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ​ caused a loss of points; in this project it is allowed by the autograder (you will need iomanip​&nbsp;&nbsp;&nbsp;&nbsp; to set the digits of precision for the median output).​

<h1>Appendix B: Tips (mostly PairingPQ, but others also)</h1>
There are helpful videos on the EECS 281 YouTube channel, specifically the running median:

<a href="https://youtu.be/_T63Cajeyhw">https://youtu.be/_T63Cajeyhw</a> <u>​ </u>(which is used for many different versions of Project 2).&nbsp; Here is a video about the Mine Escape: <a href="https://youtu.be/ICgHr6ZbUDk">https://youtu.be/ICgHr6ZbUD</a><u>​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </u><a href="https://youtu.be/ICgHr6ZbUDk">k</a>.&nbsp; Here is a video all about Part B:​&nbsp;&nbsp;&nbsp;&nbsp; <a href="https://youtu.be/kOqzBMvxfuw">https://youtu.be/kOqzBMvxfuw</a><a href="https://youtu.be/kOqzBMvxfuw">.</a><u>​</u>&nbsp; There’s also a video recorded a few years ago by a student (during office hours) about the Pairing PQ: <a href="https://youtu.be/irsHBpw2fhE">https://youtu.be/irsHBpw2fh</a>​&nbsp;&nbsp;&nbsp;&nbsp; <a href="https://youtu.be/irsHBpw2fhE">E</a><a href="https://youtu.be/irsHBpw2fhE">.</a><u>​</u>

Start coding the mine escape first, but keep thinking about the priority queue implementations.&nbsp; When you code them, the suggested order is SortedPQ, BinaryPQ, PairingPQ.

When you’re working on statistics output, be efficient.&nbsp; You can use something from this project&nbsp; to make the easiest/hardest tiles cleared more efficient.

You will need TWO priority queues in Part A: one for things discovered, and another to handle the TNT chain explosion.&nbsp; Remember, once a TNT explosion starts, it must finish!

For Part A, resist the urge to use pointers!&nbsp; If you point to somewhere within a 2D vector, how do you know it’s row and column number for printing?&nbsp; Trust us when we say that you’ll get enough pointers in the PairingPQ.

You can always count on the UnorderedPQ.h​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; being correct.&nbsp; If your ​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; testPQ.cpp​&nbsp; works with this​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; and doesn’t work with one of your other PQ implementations, it is most likely a bug in that PQ implementation.

Make sure ALL of your constructors initialize ALL of your member variables (but objects like a ​vector might be fine with just being default-constructed).&nbsp; This is most likely to be a problem with Pairing, but check the others also.

Even if you think it’s working, run your Pairing Heap with valgrind to check for memory errors and/or leaks.&nbsp; This is good advice for the entire project.

Verbose mode doesn’t require a lot of extra work and can make it easier to debug your program.&nbsp; For example, if a tile gets blown up in the wrong order, it would be very useful to know that right away, rather than wondering why the summary line has the wrong number of tiles or rubble cleared.

When you are writing a derived class and want to use the ​compare​ member variable (that is already declared in the base class), you must use ​this-&gt;compare​.&nbsp; This is because you are working on a templated class that inherits from a templated class (referred to in C++ terms as a dependent context).

Your comparator should always answer the same question!&nbsp; If called with two parameters (let’s say a, b), it should return ​true​ if: priority(a) &lt; priority(b).

Make sure that each of your PQ implementation files contains every ​#include​ needed by that file!

You might be including ​deque​ from your ​main.cpp​, and counting on that file existing for

PairingPQ.h​.&nbsp; You would then be unable to compile when we test your PQ implementations with our

.cpp​ file.

<strong>The rest of these tips are specific to the Pairing Heap. </strong>

After you’re done reading about the Pairing Heap data structure, plan on several days of coding, testing, and optimizing JUST for ​PairingPQ.h​.

<strong>DON’T USE RECURSION</strong>​, it’s very easy to have a large pairing heap that causes a stack overflow.

You can add other private member variables and functions, such as the current size and a ​meld() function.

You are not allowed to change from sibling and child pointers to a deque or vector of children pointers. You don’t want to: this is slower than using sibling/child., and the autograder timings are based on the sibling/child approach.

You are allowed to add one more pointer to the ​Node​ structure.&nbsp; You can use either a parent (pointing up) or a previous (points left except leftmost points to parent).&nbsp; You can also add a public function to return it if you want to.&nbsp; We didn’t put this variable or function in the starter file because some students want parent, some want previous.&nbsp; Neither is strictly a better choice than the other; each makes some part of Pairing harder, some part easier; both can pass the timings.

Pointers passed to ​meld()​ must each point to the “root” node of a Pairing Heap.&nbsp; Root nodes never have siblings!&nbsp; This is important to making ​meld()​ as simple and as fast as it should be.

Don’t write a copy constructor and copy the code for ​operator=()​!&nbsp; Use the copy-swap method outlined in the “Arrays and Containers” lecture.

You are allowed to write an extra function, such as ​print()​ to display the entire pairing heap, and only use it for testing.

When you need to traverse an entire pairing heap (print, copy constructor, destructor, etc.), think about the Project 1 approach!&nbsp; Use a deque, add the “starting location”, while it’s not empty take the “next” one out, add things nearby, do something with the “next” one that you took out, etc.

<h1>Appendix C: Autograder Information</h1>
The test cases for ​<strong>Part A</strong>​ on the autograder (that show in the table) are for part A, and have the following naming convention:

<ul>
<li>“INV”:
<ul>
<li>The test case is an invalid input file. Your solution should ​exit(1)​ because of an error.</li>
</ul>
</li>
<li>First letter (for anything not invalid):
<ul>
<li>‘M’ (medium), ‘L’ (large), and ‘XL’ (extra-large) denote the size of the test case.</li>
</ul>
</li>
</ul>
○&nbsp;&nbsp;&nbsp; ‘S’ indicates that the test is the one given in this spec (see Full I/O Example).

○&nbsp;&nbsp;&nbsp; ‘E’ indicates that the test case is some sort of hand-written edge case.

○&nbsp;&nbsp;&nbsp; ‘R’ indicates that the grid contains only rubble (possibly 0s, but never any TNT)..

○&nbsp;&nbsp;&nbsp; ‘N’ indicates that the grid contains no rubble or TNT (i.e. it’s all 0s).

○&nbsp;&nbsp;&nbsp; ‘T’ indicates that the grid is made entirely of TNT squares.

<ul>
<li>Second letter:
<ul>
<li>‘M’ denotes map input format and ‘R’ denotes pseudo-random input format.</li>
</ul>
</li>
<li>Lower case letters after a hyphen:
<ul>
<li>‘m’: The test is run with the median flag on.</li>
</ul>
</li>
</ul>
○&nbsp;&nbsp;&nbsp; ‘v’: The test is run with the verbose flag on.

○&nbsp;&nbsp;&nbsp; ‘s’: The test is run with the statistics flag on.

&nbsp;

When you start submitting test files to the autograder, it will tell you (in the section called “Scoring student test files”) how many bugs exist, the number needed to start earning points, and the number needed for full points.&nbsp; It will also tell you how many are needed to start earning an extra submit/day!

&nbsp;

For ​<strong>Part B</strong>​, when your priority queues (​SortedPQ​, ​BinaryPQ​, and ​PairingPQ​) are compiled with our main()​, we will perform unit testing on your data structures.&nbsp; These test cases all have three-letter names:

<ul>
<li>First letter: ​<strong>B</strong>​inary PQ, ​<strong>S</strong>​orted PQ, <strong>P</strong>​ ​airing PQ</li>
<li>Second letter: ​<strong>P</strong>​ush, ​<strong>R</strong>​ange, ​<strong>U</strong>​pdate priorities, <strong>A</strong>​ddnode,​ update​<strong>E</strong>​lt, ​<strong>C</strong>opy​ constructor, <strong>O</strong>​​perator =</li>
<li>Third letter: <strong>S</strong>​ mall, ​ <strong>M</strong>​ edium, ​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>L</strong>​ arge, e​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>X</strong>​ tra-large​</li>
</ul>
&nbsp;

A “push” test uses the .push()​ member function to insert numerous values into your priority queue. After that, the values will be checked via .top()​ and .pop()​ until the container is empty, to make sure that every value came out in the correct order. If the “push” test goes over on time, it <em>might</em>​ be the fault of your .pop()​ ,​ not your .push()​ ,​ because both must be called to verify that your container works properly.

&nbsp;

A “range” test uses the range-based constructor, from [​ start, end) to insert values into your container, then the test proceeds as described above for the “push” test. The start iterator is inclusive while the end is exclusive, as is normal for the STL.

&nbsp;

The “update priorities” tests use .push()​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; to fill your container, then half of the values that were given to you are modified (hint, this is accomplished with pointers). After .updatePriorities()​&nbsp;&nbsp; is called, all of the values are popped out and tested as above.

&nbsp;

The first three tests above are run for every priority queue type. The ones below are run only on the PairingPQ.​

&nbsp;

The “addNode” tests use .addNode()​ to fill the container instead of .push()​ ,​ and every value is checked through the returned pointer to make sure that it matches.

&nbsp;

The “updateElt” tests use .addNode()​ to fill the container, then half of the values have their priority increased by a random amount using .updateElt()​ .​ After that, values are popped off one at a time, checking to make sure that each value is correct.

&nbsp;

The “copy constructor” and “operator=” tests first fill one PairingPQ​ using .push()​ .​ Then they use the stated method to create a second PairingPQ​ from the first. Lastly every value is popped from <strong>both</strong>​ priority queues, making sure that every value is correct (and thus ensuring that a deep copy was performed, not a shallow copy).

&nbsp;

For the Pairing Heap, the .addNode()​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; member function makes a promise: the item that was added will​ ALWAYS live at the pointer returned, until the user removes it via .pop()​ (or the destructor).&nbsp; When​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; implementing .updateElt()​&nbsp; and ​&nbsp;&nbsp;&nbsp;&nbsp; .updatePriorities()​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; , you cannot delete existing nodes and create​&nbsp; new ones, as this would break the promise made by .addNode()​&nbsp; !​&nbsp; You must move nodes around.
