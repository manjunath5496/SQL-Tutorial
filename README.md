<p><strong>SQL</strong>&nbsp;(<strong>Structured Query Language</strong>)&nbsp;is a&nbsp;<a title="Domain-specific language" href="https://en.wikipedia.org/wiki/Domain-specific_language">domain-specific language</a>&nbsp;used in programming and designed for managing data held in a&nbsp;<a class="mw-redirect" title="Relational database management system" href="https://en.wikipedia.org/wiki/Relational_database_management_system">relational database management system</a>&nbsp;(RDBMS), or for stream processing in a&nbsp;<a title="Relational data stream management system" href="https://en.wikipedia.org/wiki/Relational_data_stream_management_system">relational data stream management system</a>&nbsp;(RDSMS). It is particularly useful in handling&nbsp;<a title="Data model" href="https://en.wikipedia.org/wiki/Data_model">structured data</a>, i.e. data incorporating relations among entities and variables.</p>
<p>SQL offers two main advantages over older read&ndash;write&nbsp;<a class="mw-redirect" title="API" href="https://en.wikipedia.org/wiki/API">APIs</a>&nbsp;such as&nbsp;<a title="ISAM" href="https://en.wikipedia.org/wiki/ISAM">ISAM</a>&nbsp;or&nbsp;<a class="mw-redirect" title="VSAM" href="https://en.wikipedia.org/wiki/VSAM">VSAM</a>. Firstly, it introduced the concept of accessing many records with one single command. Secondly, it eliminates the need to specify&nbsp;<em>how</em>&nbsp;to reach a record, e.g. with or without an&nbsp;<a title="Database index" href="https://en.wikipedia.org/wiki/Database_index">index</a>.</p>
<p>Originally based upon&nbsp;<a title="Relational algebra" href="https://en.wikipedia.org/wiki/Relational_algebra">relational algebra</a>&nbsp;and&nbsp;<a title="Tuple relational calculus" href="https://en.wikipedia.org/wiki/Tuple_relational_calculus">tuple relational calculus</a>, SQL consists of many types of statements,&nbsp;which may be informally classed as&nbsp;<a title="Sublanguage" href="https://en.wikipedia.org/wiki/Sublanguage">sublanguages</a>, commonly: a&nbsp;<a class="mw-redirect" title="Data query language" href="https://en.wikipedia.org/wiki/Data_query_language">data query language</a>&nbsp;(DQL),&nbsp;a&nbsp;<a title="Data definition language" href="https://en.wikipedia.org/wiki/Data_definition_language">data definition language</a>&nbsp;(DDL),<sup id="cite_ref-10" class="reference"><a href="https://en.wikipedia.org/wiki/SQL#cite_note-10">[b]</a></sup>&nbsp;a&nbsp;<a title="Data control language" href="https://en.wikipedia.org/wiki/Data_control_language">data control language</a>&nbsp;(DCL), and a&nbsp;<a title="Data manipulation language" href="https://en.wikipedia.org/wiki/Data_manipulation_language">data manipulation language</a>&nbsp;(DML).&nbsp;The scope of SQL includes data query, data manipulation (insert, update and delete), data definition (<a title="Database schema" href="https://en.wikipedia.org/wiki/Database_schema">schema</a>&nbsp;creation and modification), and data access control. Although SQL is essentially a&nbsp;<a title="Declarative programming" href="https://en.wikipedia.org/wiki/Declarative_programming">declarative language</a>&nbsp;(<a class="mw-redirect" title="4GL" href="https://en.wikipedia.org/wiki/4GL">4GL</a>), it includes also&nbsp;<a title="Procedural programming" href="https://en.wikipedia.org/wiki/Procedural_programming">procedural</a>&nbsp;elements.</p>
<p>SQL was one of the first commercial languages to utilize&nbsp;<a title="Edgar F. Codd" href="https://en.wikipedia.org/wiki/Edgar_F._Codd">Edgar F. Codd</a>&rsquo;s&nbsp;<a title="Relational model" href="https://en.wikipedia.org/wiki/Relational_model">relational model</a>. The model was described in his influential 1970 paper, "A Relational Model of Data for Large Shared Data Banks".&nbsp;Despite not entirely adhering to&nbsp;<a title="Codd's 12 rules" href="https://en.wikipedia.org/wiki/Codd%27s_12_rules">the relational model as described by Codd</a>, it became the most widely used database language.</p>
<p>SQL became a&nbsp;<a title="Technical standard" href="https://en.wikipedia.org/wiki/Technical_standard">standard</a>&nbsp;of the&nbsp;<a title="American National Standards Institute" href="https://en.wikipedia.org/wiki/American_National_Standards_Institute">American National Standards Institute</a>&nbsp;(ANSI) in 1986, and of the&nbsp;<a title="International Organization for Standardization" href="https://en.wikipedia.org/wiki/International_Organization_for_Standardization">International Organization for Standardization</a>&nbsp;(ISO) in 1987.&nbsp;Since then, the standard has been revised to include a larger set of features. Despite the existence of such standards, most SQL code is not completely portable among different database systems without adjustments.</p>


</br>

<div class="toctitle" dir="ltr" lang="en">
<h2 id="mw-toc-heading">Contents</h2>
<label class="toctogglelabel" for="toctogglecheckbox"></label></div>
<ul>
<li class="toclevel-1 tocsection-1"><a href="#History"><span class="toctext">History</span></a></li>
<li class="toclevel-1 tocsection-2"><a href="#Design"><span class="toctext">Design</span></a></li>
<li class="toclevel-1 tocsection-3"><a href="#Syntax"><span class="toctext">Syntax</span></a></li>
<li class="toclevel-1 tocsection-4"><a href="#Procedural_extensions"><span class="toctext">Procedural extensions</span></a></li>
<li class="toclevel-1 tocsection-5"><a href="#Interoperability_and_standardization"><span class="toctext">Interoperability and standardization</span></a></li>
<li class="toclevel-1 tocsection-6"><a href="#Alternatives"><span class="toctext">Alternatives</span></a></li>
<li class="toclevel-1 tocsection-7"><a href="#Distributed_SQL_processing"><span class="toctext">Distributed SQL processing</span></a></li>
<li class="toclevel-1 tocsection-8"><a href="#Criticisms"><span class="toctext">Criticisms</span></a>
<ul>
<li class="toclevel-2 tocsection-9"><a href="#Orthogonality_and_completeness"><span class="toctext">Orthogonality and completeness</span></a></li>
<li class="toclevel-2 tocsection-10"><a href="#NULLs"><span class="toctext">NULLs</span></a></li>
<li class="toclevel-2 tocsection-11"><a href="#Duplicates"><span class="toctext">Duplicates</span></a></li>
<li class="toclevel-2 tocsection-12"><a href="#Impedance_mismatch"><span class="toctext">Impedance mismatch</span></a></li>
</ul>
</li>
          
<li class="toclevel-1 tocsection-13"><a href="#Books"><span class="toctext">Books</span></a></li>          
</ul>

</br>


<h2><span id="History" class="mw-headline">History</span></h2>

</br>

<table class="infobox biography vcard">
<tbody>
<tr>
<td><a class="image" href="Edgar_F_Codd.jpg"><img src="Edgar_F_Codd.jpg" srcset="Edgar_F_Codd.jpg" alt="Edgar F Codd.jpg" width="150" height="213" data-file-width="211" data-file-height="300" /></a></td>
</tr>
<tr>
<td>
<div class="nickname" style="text-align: center;"><strong>Edgar Frank Codd</strong></div>
<br /><br /></td>
</tr>
</tbody>
</table>

</br>
<h2>Publications </h2>
<ul>
 <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(58).pdf" style="text-decoration:none;">Relational Database: A Practical Foundation for Productivity</a></li>
                            
 <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(59).pdf" style="text-decoration:none;">Cellular Automata</a></li>

<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(60).pdf" style="text-decoration:none;">A Relational Model of Data for Large Shared Data Banks</a></li>
 <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(61).pdf" style="text-decoration:none;">Relational Completeness of Data Base Sublanguages</a></li>                              
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(62).pdf" style="text-decoration:none;">Extending the Database Relational Model to Capture More Meaning</a></li>
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(63).pdf" style="text-decoration:none;">Multiprogramming STRETCH: feasibility considerations</a></li>
 <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(64).pdf" style="text-decoration:none;">Derivability, Redundancy and Consistency of Relations Stored in Large Data Banks</a></li>                              
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(65).rar" style="text-decoration:none;">The Relational Model for Database Management: Version 2 </a></li>
</ul>
</br>
<p>SQL was initially developed at&nbsp;<a title="IBM" href="https://en.wikipedia.org/wiki/IBM">IBM</a>&nbsp;by&nbsp;<a title="Donald D. Chamberlin" href="https://en.wikipedia.org/wiki/Donald_D._Chamberlin">Donald D. Chamberlin</a>&nbsp;and&nbsp;<a title="Raymond F. Boyce" href="https://en.wikipedia.org/wiki/Raymond_F._Boyce">Raymond F. Boyce</a>&nbsp;after learning about the relational model from&nbsp;<a class="mw-redirect" title="Ted Codd" href="https://en.wikipedia.org/wiki/Ted_Codd">Ted Codd</a>&nbsp;in the early 1970s.&nbsp;This version, initially called&nbsp;<em>SEQUEL</em>&nbsp;(<em>Structured English Query Language</em>), was designed to manipulate and retrieve data stored in IBM's original quasi-relational database management system,&nbsp;<a title="IBM System R" href="https://en.wikipedia.org/wiki/IBM_System_R">System R</a>, which a group at&nbsp;<a class="mw-redirect" title="IBM Almaden Research Center" href="https://en.wikipedia.org/wiki/IBM_Almaden_Research_Center">IBM San Jose Research Laboratory</a>&nbsp;had developed during the 1970s.</p>
<p>Chamberlin and Boyce's first attempt of a relational database language was Square, but it was difficult to use due to subscript notation. After moving to the San Jose Research Laboratory in 1973, they began work on SEQUEL.&nbsp;The acronym SEQUEL was later changed to SQL because "SEQUEL" was a&nbsp;<a title="Trademark" href="https://en.wikipedia.org/wiki/Trademark">trademark</a>&nbsp;of the&nbsp;<a title="United Kingdom" href="https://en.wikipedia.org/wiki/United_Kingdom">UK-based</a>&nbsp;<a title="Hawker Siddeley" href="https://en.wikipedia.org/wiki/Hawker_Siddeley">Hawker Siddeley</a>&nbsp;Dynamics Engineering Limited company.</p>
<p>After testing SQL at customer test sites to determine the usefulness and practicality of the system, IBM began developing commercial products based on their System R prototype including&nbsp;<a title="IBM System/38" href="https://en.wikipedia.org/wiki/IBM_System/38">System/38</a>,&nbsp;<a title="IBM SQL/DS" href="https://en.wikipedia.org/wiki/IBM_SQL/DS">SQL/DS</a>, and&nbsp;<a class="mw-redirect" title="IBM DB2" href="https://en.wikipedia.org/wiki/IBM_DB2">DB2</a>, which were commercially available in 1979, 1981, and 1983, respectively.</p>
<p>In the late 1970s, Relational Software, Inc. (now&nbsp;<a title="Oracle Corporation" href="https://en.wikipedia.org/wiki/Oracle_Corporation">Oracle Corporation</a>) saw the potential of the concepts described by Codd, Chamberlin, and Boyce, and developed their own SQL-based&nbsp;<a title="Relational database" href="https://en.wikipedia.org/wiki/Relational_database">RDMS</a>&nbsp;with aspirations of selling it to the&nbsp;<a title="United States Navy" href="https://en.wikipedia.org/wiki/United_States_Navy">U.S. Navy</a>,&nbsp;<a title="Central Intelligence Agency" href="https://en.wikipedia.org/wiki/Central_Intelligence_Agency">Central Intelligence Agency</a>, and other&nbsp;<a title="Federal government of the United States" href="https://en.wikipedia.org/wiki/Federal_government_of_the_United_States">U.S. government</a>&nbsp;agencies. In June 1979, Relational Software, Inc. introduced the first commercially available implementation of SQL,&nbsp;<a title="Oracle Database" href="https://en.wikipedia.org/wiki/Oracle_Database">Oracle</a>&nbsp;V2 (Version2) for&nbsp;<a title="VAX" href="https://en.wikipedia.org/wiki/VAX">VAX</a>&nbsp;computers.</p>
<p>By 1986,&nbsp;<a class="mw-redirect" title="ANSI" href="https://en.wikipedia.org/wiki/ANSI">ANSI</a>&nbsp;and&nbsp;<a class="mw-redirect" title="ISO" href="https://en.wikipedia.org/wiki/ISO">ISO</a>&nbsp;standard groups officially adopted the standard "Database Language SQL" language definition. New versions of the standard were published in 1989, 1992, 1996, 1999, 2003, 2006, 2008, 2011&nbsp;and, most recently, 2016.</p>
<h2><span id="Design" class="mw-headline">Design</span></h2>
<p>SQL deviates in several ways from its theoretical foundation, the&nbsp;<a title="Relational model" href="https://en.wikipedia.org/wiki/Relational_model">relational model</a>&nbsp;and its&nbsp;<a title="Tuple relational calculus" href="https://en.wikipedia.org/wiki/Tuple_relational_calculus">tuple calculus</a>. In that model, a table is a&nbsp;<a title="Set (mathematics)" href="https://en.wikipedia.org/wiki/Set_(mathematics)">set</a>&nbsp;of tuples, while in SQL, tables and query results are&nbsp;<a class="mw-redirect" title="List (computing)" href="https://en.wikipedia.org/wiki/List_(computing)">lists</a>&nbsp;of rows: the same row may occur multiple times, and the order of rows can be employed in queries (e.g. in the LIMIT clause).</p>
<p>Critics argue that SQL should be replaced with a language that returns strictly to the original foundation: for example, see&nbsp;<em><a title="The Third Manifesto" href="https://en.wikipedia.org/wiki/The_Third_Manifesto">The Third Manifesto</a></em>. However, no known proof exists that such uniqueness cannot be added to SQL itself, or at least a variation of SQL. In other words, it's quite possible that SQL can be "fixed" or at least improved in this regard such that the industry may not have to switch to a completely different query language to obtain uniqueness. Debate on this remains open.</p>

<h2><span id="Syntax" class="mw-headline">Syntax</span></h2>


<p>The&nbsp;<a title="Syntax (programming languages)" href="https://en.wikipedia.org/wiki/Syntax_(programming_languages)">syntax</a>&nbsp;of the&nbsp;<a title="SQL" href="https://en.wikipedia.org/wiki/SQL">SQL</a>&nbsp;programming language is defined and maintained by&nbsp;<a title="ISO/IEC JTC 1/SC 32" href="https://en.wikipedia.org/wiki/ISO/IEC_JTC_1/SC_32">ISO/IEC SC 32</a>&nbsp;as part of&nbsp;<em>ISO/IEC 9075</em>. This standard is not freely available. Despite the existence of the standard, SQL code is not completely portable among different database systems without adjustments.</p>
<div class="toctitle" dir="ltr" lang="en">
<h2 id="mw-toc-heading">Contents</h2>
<label class="toctogglelabel" for="toctogglecheckbox"></label></div>
<ul>
<li class="toclevel-1 tocsection-1"><a href="#Language_elements"><span class="toctext">Language elements</span></a></li>
<li class="toclevel-1 tocsection-2"><a href="#Operators"><span class="toctext">Operators</span></a></li>
<li class="toclevel-1 tocsection-3"><a href="#Comments"><span class="toctext">Comments</span></a></li>
<li class="toclevel-1 tocsection-4"><a href="#Queries"><span class="toctext">Queries</span></a>
<ul>
<li class="toclevel-2 tocsection-5"><a href="#Subqueries"><span class="toctext">Subqueries</span></a></li>
<li class="toclevel-2 tocsection-6"><a href="#Derived_table"><span class="toctext">Derived table</span></a></li>
<li class="toclevel-2 tocsection-7"><a href="#Null_or_three-valued_logic_(3VL)"><span class="toctext">Null or three-valued logic (3VL)</span></a></li>
<li class="toclevel-2 tocsection-8"><a href="#Data_manipulation"><span class="toctext">Data manipulation</span></a></li>
<li class="toclevel-2 tocsection-9"><a href="#Transaction_controls"><span class="toctext">Transaction controls</span></a></li>
<li class="toclevel-2 tocsection-10"><a href="#Data_definition"><span class="toctext">Data definition</span></a></li>
<li class="toclevel-2 tocsection-11"><a href="#Data_types"><span class="toctext">Data types</span></a></li>
<li class="toclevel-2 tocsection-12"><a href="#Data_control"><span class="toctext">Data control</span></a></li>
</ul>
</li>
</ul>
</br>
<h2><span id="Language_elements" class="mw-headline">Language elements</span></h2>
<p>&nbsp;</p>
<div class="thumb tright">
<div class="thumbinner">
<div class="thumbimage noresize"><span class="mwe-math-element"><img class="mwe-math-fallback-image-inline" src="sql.png" alt="SQL" /></span></div>
<div class="thumbcaption">&nbsp;</div>
<div class="thumbcaption"><strong>A chart showing several of the SQL language elements that compose a single statement. This adds one to the population of the USA in the country table.</strong></div>
<div class="thumbcaption">&nbsp;</div>
<div class="thumbcaption">&nbsp;</div>
</div>
</div>
<p>The SQL language is subdivided into several language elements, including:</p>
<ul>
<li><em>Clauses</em>, which are constituent components of statements and queries. (In some cases, these are optional.)</li>
<li><em>Expressions</em>, which can produce either&nbsp;<a class="mw-redirect" title="Scalar (computing)" href="https://en.wikipedia.org/wiki/Scalar_(computing)">scalar</a>&nbsp;values, or&nbsp;<a title="Table (database)" href="https://en.wikipedia.org/wiki/Table_(database)">tables</a>&nbsp;consisting of&nbsp;<a title="Column (database)" href="https://en.wikipedia.org/wiki/Column_(database)">columns</a>&nbsp;and&nbsp;<a title="Row (database)" href="https://en.wikipedia.org/wiki/Row_(database)">rows</a>&nbsp;of data</li>
<li><em>Predicates</em>, which specify conditions that can be evaluated to SQL&nbsp;<a class="mw-redirect" title="Ternary logic" href="https://en.wikipedia.org/wiki/Ternary_logic">three-valued logic (3VL)</a>&nbsp;(true/false/unknown) or&nbsp;<a class="mw-redirect" title="Boolean logic" href="https://en.wikipedia.org/wiki/Boolean_logic">Boolean</a>&nbsp;<a title="Truth value" href="https://en.wikipedia.org/wiki/Truth_value">truth values</a>&nbsp;and are used to limit the effects of statements and queries, or to change program flow.</li>
<li><em>Queries</em>, which retrieve the data based on specific criteria. This is an important element of&nbsp;<em>SQL</em>.</li>
<li><em>Statements</em>, which may have a persistent effect on schemata and data, or may control transactions, program flow, connections, sessions, or diagnostics.
<ul>
<li>SQL statements also include the&nbsp;<a title="Semicolon" href="https://en.wikipedia.org/wiki/Semicolon">semicolon</a>&nbsp;(";") statement terminator. Though not required on every platform, it is defined as a standard part of the SQL grammar.</li>
</ul>
</li>
<li><em><a class="mw-redirect" title="Whitespace (computer science)" href="https://en.wikipedia.org/wiki/Whitespace_(computer_science)">Insignificant whitespace</a></em>&nbsp;is generally ignored in SQL statements and queries, making it easier to format SQL code for readability.</li>
</ul>
<h2><span id="Operators" class="mw-headline">Operators</span></h2>
<table class="wikitable">
<tbody>
<tr>
<th>Operator</th>
<th>Description</th>
<th>Example</th>
</tr>
<tr>
<td><code>=</code></td>
<td>Equal to</td>
<td><code id="" class="mw-highlight" dir="ltr"><span class="n">Author</span>&nbsp;<span class="o">=</span>&nbsp;<span class="s1">'Alcott'</span></code></td>
</tr>
<tr>
<td><code>&lt;&gt;</code></td>
<td>Not equal to (many DBMSs accept&nbsp;<code>!=</code>&nbsp;in addition to&nbsp;<code>&lt;&gt;</code>)</td>
<td><code id="" class="mw-highlight" dir="ltr"><span class="n">Dept</span>&nbsp;<span class="o">&lt;&gt;</span>&nbsp;<span class="s1">'Sales'</span></code></td>
</tr>
<tr>
<td><code>&gt;</code></td>
<td>Greater than</td>
<td><code id="" class="mw-highlight" dir="ltr"><span class="n">Hire_Date</span>&nbsp;<span class="o">&gt;</span>&nbsp;<span class="s1">'2012-01-31'</span></code></td>
</tr>
<tr>
<td><code>&lt;</code></td>
<td>Less than</td>
<td><code id="" class="mw-highlight" dir="ltr"><span class="n">Bonus</span>&nbsp;<span class="o">&lt;</span>&nbsp;<span class="mi">50000</span><span class="p">.</span><span class="mi">00</span></code></td>
</tr>
<tr>
<td><code>&gt;=</code></td>
<td>Greater than or equal</td>
<td><code id="" class="mw-highlight" dir="ltr"><span class="n">Dependents</span>&nbsp;<span class="o">&gt;=</span>&nbsp;<span class="mi">2</span></code></td>
</tr>
<tr>
<td><code>&lt;=</code></td>
<td>Less than or equal</td>
<td><code id="" class="mw-highlight" dir="ltr"><span class="n">Rate</span>&nbsp;<span class="o">&lt;=</span>&nbsp;<span class="mi">0</span><span class="p">.</span><span class="mi">05</span></code></td>
</tr>
<tr>
<td><a title="Where (SQL)" href="https://en.wikipedia.org/wiki/Where_(SQL)#BETWEEN"><code id="" class="mw-highlight" dir="ltr"><span class="k">BETWEEN</span></code></a></td>
<td>Between an inclusive range</td>
<td><code id="" class="mw-highlight" dir="ltr"><span class="n">Cost</span>&nbsp;<span class="k">BETWEEN</span>&nbsp;<span class="mi">100</span><span class="p">.</span><span class="mi">00</span>&nbsp;<span class="k">AND</span>&nbsp;<span class="mi">500</span><span class="p">.</span><span class="mi">00</span></code></td>
</tr>
<tr>
<td rowspan="2"><a class="mw-redirect" title="Like (SQL)" href="https://en.wikipedia.org/wiki/Like_(SQL)"><code id="" class="mw-highlight" dir="ltr"><span class="k">LIKE</span></code></a></td>
<td>Begins with a character pattern</td>
<td><code id="" class="mw-highlight" dir="ltr"><span class="n">Full_Name</span>&nbsp;<span class="k">LIKE</span>&nbsp;<span class="s1">'Will%'</span></code></td>
</tr>
<tr>
<td>Contains a character pattern</td>
<td><code id="" class="mw-highlight" dir="ltr"><span class="n">Full_Name</span>&nbsp;<span class="k">LIKE</span>&nbsp;<span class="s1">'%Will%'</span></code></td>
</tr>
<tr>
<td><a title="Where (SQL)" href="https://en.wikipedia.org/wiki/Where_(SQL)#IN"><code id="" class="mw-highlight" dir="ltr"><span class="p">[</span><span class="k">NOT</span><span class="p">]</span>&nbsp;<span class="k">IN</span></code></a></td>
<td>Equal to one of multiple possible values</td>
<td><code id="" class="mw-highlight" dir="ltr"><span class="n">DeptCode</span>&nbsp;<span class="k">IN</span>&nbsp;<span class="p">(</span><span class="mi">101</span><span class="p">,</span>&nbsp;<span class="mi">103</span><span class="p">,</span>&nbsp;<span class="mi">209</span><span class="p">)</span></code></td>
</tr>
<tr>
<td><a title="SQL syntax" href="https://en.wikipedia.org/wiki/SQL_syntax#Null_or_three-valued_logic_(3VL)"><code id="" class="mw-highlight" dir="ltr"><span class="k">IS</span>&nbsp;<span class="p">[</span><span class="k">NOT</span><span class="p">]</span>&nbsp;<span class="k">NULL</span></code></a></td>
<td>Compare to null (missing data)</td>
<td><code id="" class="mw-highlight" dir="ltr"><span class="n">Address</span>&nbsp;<span class="k">IS</span>&nbsp;<span class="k">NOT</span>&nbsp;<span class="k">NULL</span></code></td>
</tr>
<tr>
<td><code id="" class="mw-highlight" dir="ltr"><span class="k">IS</span>&nbsp;<span class="p">[</span><span class="k">NOT</span><span class="p">]</span>&nbsp;<span class="k">TRUE</span></code>&nbsp;<em>or</em>&nbsp;<code id="" class="mw-highlight" dir="ltr"><span class="k">IS</span>&nbsp;<span class="p">[</span><span class="k">NOT</span><span class="p">]</span>&nbsp;<span class="k">FALSE</span></code></td>
<td>Boolean truth value test</td>
<td><code id="" class="mw-highlight" dir="ltr"><span class="n">PaidVacation</span>&nbsp;<span class="k">IS</span>&nbsp;<span class="k">TRUE</span></code></td>
</tr>
<tr>
<td><a title="SQL syntax" href="https://en.wikipedia.org/wiki/SQL_syntax#Null_or_three-valued_logic_(3VL)"><code id="" class="mw-highlight" dir="ltr"><span class="k">IS</span>&nbsp;<span class="k">NOT</span>&nbsp;<span class="k">DISTINCT</span>&nbsp;<span class="k">FROM</span></code></a></td>
<td>Is equal to value or both are nulls (missing data)</td>
<td><code id="" class="mw-highlight" dir="ltr"><span class="n">Debt</span>&nbsp;<span class="k">IS</span>&nbsp;<span class="k">NOT</span>&nbsp;<span class="k">DISTINCT</span>&nbsp;<span class="k">FROM</span>&nbsp;<span class="o">-</span>&nbsp;<span class="n">Receivables</span></code></td>
</tr>
<tr>
<td><code id="" class="mw-highlight" dir="ltr"><span class="k">AS</span></code></td>
<td>Used to change a column name when viewing results</td>
<td><code id="" class="mw-highlight" dir="ltr"><span class="k">SELECT</span>&nbsp;<span class="n">employee</span>&nbsp;<span class="k">AS</span>&nbsp;<span class="ss">"department1"</span></code></td>
</tr>
</tbody>
</table>
<p>Other operators have at times been suggested or implemented, such as the&nbsp;<a title="Skyline operator" href="https://en.wikipedia.org/wiki/Skyline_operator">skyline operator</a>&nbsp;(for finding only those rows that are not 'worse' than any others).</p>
<p><span id="Conditional_(CASE)_expressions"></span>SQL has the&nbsp;<code>case</code>&nbsp;expression, which was introduced in&nbsp;<a title="SQL-92" href="https://en.wikipedia.org/wiki/SQL-92">SQL-92</a>. In its most general form, which is called a "searched case" in the SQL standard:</p>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">CASE</span> <span class="k">WHEN</span> <span class="n">n</span> <span class="o">&gt;</span> <span class="mi">0</span>
          <span class="k">THEN</span> <span class="s1">'positive'</span>
     <span class="k">WHEN</span> <span class="n">n</span> <span class="o">&lt;</span> <span class="mi">0</span>
          <span class="k">THEN</span> <span class="s1">'negative'</span>
     <span class="k">ELSE</span> <span class="s1">'zero'</span>
<span class="k">END</span>
</pre>
</div>
<p>SQL tests&nbsp;<code>WHEN</code>&nbsp;conditions in the order they appear in the source. If the source does not specify an&nbsp;<code>ELSE</code>&nbsp;expression, SQL defaults to&nbsp;<code>ELSE NULL</code>. An abbreviated syntax called "simple case" can also be used:</p>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">CASE</span> <span class="n">n</span> <span class="k">WHEN</span> <span class="mi">1</span>
            <span class="k">THEN</span> <span class="s1">'One'</span>
       <span class="k">WHEN</span> <span class="mi">2</span>
            <span class="k">THEN</span> <span class="s1">'Two'</span>
       <span class="k">ELSE</span> <span class="s1">'I cannot count that high'</span>
<span class="k">END</span>
</pre>
</div>
<p>This syntax uses implicit equality comparisons, with&nbsp;<a class="mw-redirect" title="SQL CASE" href="https://en.wikipedia.org/wiki/SQL_CASE">the usual caveats for comparing with NULL</a>.</p>
<p>There are two short forms for special&nbsp;<code>CASE</code>&nbsp;expressions:&nbsp;<code>COALESCE</code>&nbsp;and&nbsp;<code>NULLIF</code>.</p>
<p>The&nbsp;<code>COALESCE</code>&nbsp;expression returns the value of the first non-NULL operand, found by working from left to right, or NULL if all the operands equal NULL.</p>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="n">COALESCE</span><span class="p">(</span><span class="n">x1</span><span class="p">,</span><span class="n">x2</span><span class="p">)</span>
</pre>
</div>
<p>is equivalent to:</p>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">CASE</span> <span class="k">WHEN</span> <span class="n">x1</span> <span class="k">IS</span> <span class="k">NOT</span> <span class="k">NULL</span> <span class="k">THEN</span> <span class="n">x1</span>
     <span class="k">ELSE</span> <span class="n">x2</span>
<span class="k">END</span>
</pre>
</div>
<p>The&nbsp;<code>NULLIF</code>&nbsp;expression has two operands and returns NULL if the operands have the same value, otherwise it has the value of the first operand.</p>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">NULLIF</span><span class="p">(</span><span class="n">x1</span><span class="p">,</span> <span class="n">x2</span><span class="p">)</span>
</pre>
</div>
<p>is equivalent to</p>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">CASE</span> <span class="k">WHEN</span> <span class="n">x1</span> <span class="o">=</span> <span class="n">x2</span> <span class="k">THEN</span> <span class="k">NULL</span> <span class="k">ELSE</span> <span class="n">x1</span> <span class="k">END</span>
</pre>
</div>
<h2><span id="Comments" class="mw-headline">Comments</span></h2>
<p>Standard SQL allows two formats for&nbsp;<a title="Comment (computer programming)" href="https://en.wikipedia.org/wiki/Comment_(computer_programming)">comments</a>:&nbsp;<code>-- comment</code>, which is ended by the first&nbsp;<a title="Newline" href="https://en.wikipedia.org/wiki/Newline">newline</a>, and&nbsp;<code>/* comment */</code>, which can span multiple lines.</p>
<h2><span id="Queries" class="mw-headline">Queries</span></h2>
<p>The most common operation in SQL, the query, makes use of the declarative&nbsp;<code><a title="Select (SQL)" href="https://en.wikipedia.org/wiki/Select_(SQL)">SELECT</a></code>&nbsp;statement.&nbsp;<code>SELECT</code>&nbsp;retrieves data from one or more&nbsp;<a title="Table (database)" href="https://en.wikipedia.org/wiki/Table_(database)">tables</a>, or expressions. Standard&nbsp;<code>SELECT</code>&nbsp;statements have no persistent effects on the database. Some non-standard implementations of&nbsp;<code>SELECT</code>&nbsp;can have persistent effects, such as the&nbsp;<code>SELECT INTO</code>&nbsp;syntax provided in some databases.</p>
<p>Queries allow the user to describe desired data, leaving the&nbsp;<a class="mw-redirect" title="Database management system" href="https://en.wikipedia.org/wiki/Database_management_system">database management system (DBMS)</a>&nbsp;to carry out&nbsp;<a title="Query plan" href="https://en.wikipedia.org/wiki/Query_plan">planning</a>,&nbsp;<a class="mw-redirect" title="Query optimizer" href="https://en.wikipedia.org/wiki/Query_optimizer">optimizing</a>, and performing the physical operations necessary to produce that result as it chooses.</p>
<p>A query includes a list of columns to include in the final result, normally immediately following the&nbsp;<code>SELECT</code>&nbsp;keyword. An asterisk ("<code>*</code>") can be used to specify that the query should return all columns of the queried tables.&nbsp;<code>SELECT</code>&nbsp;is the most complex statement in SQL, with optional keywords and clauses that include:</p>
<ul>
<li>The&nbsp;<code><a title="From (SQL)" href="https://en.wikipedia.org/wiki/From_(SQL)">FROM</a></code>&nbsp;clause, which indicates the table(s) to retrieve data from. The&nbsp;<code>FROM</code>&nbsp;clause can include optional&nbsp;<code><a title="Join (SQL)" href="https://en.wikipedia.org/wiki/Join_(SQL)">JOIN</a></code>&nbsp;subclauses to specify the rules for joining tables.</li>
<li>The&nbsp;<code><a title="Where (SQL)" href="https://en.wikipedia.org/wiki/Where_(SQL)">WHERE</a></code>&nbsp;clause includes a comparison predicate, which restricts the rows returned by the query. The&nbsp;<code>WHERE</code>&nbsp;clause eliminates all rows from the result set where the comparison predicate does not evaluate to True.</li>
<li>The&nbsp;<code>GROUP BY</code>&nbsp;clause projects rows having common values into a smaller set of rows.&nbsp;<code>GROUP BY</code>&nbsp;is often used in conjunction with SQL aggregation functions or to eliminate duplicate rows from a result set. The&nbsp;<code>WHERE</code>&nbsp;clause is applied before the&nbsp;<code>GROUP BY</code>&nbsp;clause.</li>
<li>The&nbsp;<code><a title="Having (SQL)" href="https://en.wikipedia.org/wiki/Having_(SQL)">HAVING</a></code>&nbsp;clause includes a predicate used to filter rows resulting from the&nbsp;<code>GROUP BY</code>&nbsp;clause. Because it acts on the results of the&nbsp;<code>GROUP BY</code>&nbsp;clause, aggregation functions can be used in the&nbsp;<code>HAVING</code>&nbsp;clause predicate.</li>
<li>The&nbsp;<code><a class="mw-redirect" title="Order by (SQL)" href="https://en.wikipedia.org/wiki/Order_by_(SQL)">ORDER BY</a></code>&nbsp;clause identifies which column[s] to use to sort the resulting data, and in which direction to sort them (ascending or descending). Without an&nbsp;<code>ORDER BY</code>&nbsp;clause, the order of rows returned by an SQL query is undefined.</li>
<li>The&nbsp;<code>DISTINCT</code>&nbsp;keyword&nbsp;eliminates duplicate data.</li>
<li>The&nbsp;<code>OFFSET</code>&nbsp;clause specifies the number of rows to skip before starting to return data. The&nbsp;<code>FETCH FIRST</code>&nbsp;clause specifies the number of rows to return. (Some SQL databases instead have non-standard alternatives, e.g.&nbsp;<code>LIMIT</code>,&nbsp;<code>TOP</code>&nbsp;or&nbsp;<code>ROWNUM</code>.)</li>
</ul>
<p>The clauses of a query have a particular order of execution, which is denoted by the number on the right hand side. It is as follows:</p>
<table>
<tbody>
<tr>
<td><code>SELECT&nbsp;<em>&lt;columns&gt;</em></code></td>
<td>5.</td>
</tr>
<tr>
<td><code>FROM&nbsp;<em>&lt;table&gt;</em></code></td>
<td>1.</td>
</tr>
<tr>
<td><code>WHERE&nbsp;<em>&lt;predicate on rows&gt;</em></code></td>
<td>2.</td>
</tr>
<tr>
<td><code>GROUP BY&nbsp;<em>&lt;columns&gt;</em></code></td>
<td>3.</td>
</tr>
<tr>
<td><code>HAVING&nbsp;<em>&lt;predicate on groups&gt;</em></code></td>
<td>4.</td>
</tr>
<tr>
<td><code>ORDER BY&nbsp;<em>&lt;columns&gt;</em></code></td>
<td>6.</td>
</tr>
<tr>
<td><code>OFFSET</code></td>
<td>7.</td>
</tr>
<tr>
<td><code>FETCH FIRST</code></td>
<td>8.</td>
</tr>
</tbody>
</table>
<p>The following example of a&nbsp;<code>SELECT</code>&nbsp;query returns a list of expensive books. The query retrieves all rows from the&nbsp;<em>Book</em>&nbsp;table in which the&nbsp;<em>price</em>&nbsp;column contains a value greater than 100.00. The result is sorted in ascending order by&nbsp;<em>title</em>. The asterisk (*) in the&nbsp;<em>select list</em>&nbsp;indicates that all columns of the&nbsp;<em>Book</em>&nbsp;table should be included in the result set.</p>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">SELECT</span> <span class="o">*</span>
 <span class="k">FROM</span>  <span class="n">Book</span>
 <span class="k">WHERE</span> <span class="n">price</span> <span class="o">&gt;</span> <span class="mi">100</span><span class="p">.</span><span class="mi">00</span>
 <span class="k">ORDER</span> <span class="k">BY</span> <span class="n">title</span><span class="p">;</span>
</pre>
</div>
<p>The example below demonstrates a query of multiple tables, grouping, and aggregation, by returning a list of books and the number of authors associated with each book.</p>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">SELECT</span> <span class="n">Book</span><span class="p">.</span><span class="n">title</span> <span class="k">AS</span> <span class="n">Title</span><span class="p">,</span>
       <span class="k">count</span><span class="p">(</span><span class="o">*</span><span class="p">)</span> <span class="k">AS</span> <span class="n">Authors</span>
 <span class="k">FROM</span>  <span class="n">Book</span>
 <span class="k">JOIN</span>  <span class="n">Book_author</span>
   <span class="k">ON</span>  <span class="n">Book</span><span class="p">.</span><span class="n">isbn</span> <span class="o">=</span> <span class="n">Book_author</span><span class="p">.</span><span class="n">isbn</span>
 <span class="k">GROUP</span> <span class="k">BY</span> <span class="n">Book</span><span class="p">.</span><span class="n">title</span><span class="p">;</span>
</pre>
</div>
<p>Example output might resemble the following:</p>
<pre>Title                  Authors
---------------------- -------
SQL Examples and Guide 4
The Joy of SQL         1
An Introduction to SQL 2
Pitfalls of SQL        1
</pre>
<p>Under the precondition that&nbsp;<em>isbn</em>&nbsp;is the only common column name of the two tables and that a column named&nbsp;<em>title</em>&nbsp;only exists in the&nbsp;<em>Book</em>&nbsp;table, one could re-write the query above in the following form:</p>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">SELECT</span> <span class="n">title</span><span class="p">,</span>
       <span class="k">count</span><span class="p">(</span><span class="o">*</span><span class="p">)</span> <span class="k">AS</span> <span class="n">Authors</span>
 <span class="k">FROM</span>  <span class="n">Book</span>
 <span class="k">NATURAL</span> <span class="k">JOIN</span> <span class="n">Book_author</span>
 <span class="k">GROUP</span> <span class="k">BY</span> <span class="n">title</span><span class="p">;</span>
</pre>
</div>
<p>However, many&nbsp;vendors either do not support this approach, or require certain column-naming conventions for natural joins to work effectively.</p>
<p>SQL includes operators and functions for calculating values on stored values. SQL allows the use of expressions in the&nbsp;<em>select list</em>&nbsp;to project data, as in the following example, which returns a list of books that cost more than 100.00 with an additional&nbsp;<em>sales_tax</em>&nbsp;column containing a sales tax figure calculated at 6% of the&nbsp;<em>price</em>.</p>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">SELECT</span> <span class="n">isbn</span><span class="p">,</span>
       <span class="n">title</span><span class="p">,</span>
       <span class="n">price</span><span class="p">,</span>
       <span class="n">price</span> <span class="o">*</span> <span class="mi">0</span><span class="p">.</span><span class="mi">06</span> <span class="k">AS</span> <span class="n">sales_tax</span>
 <span class="k">FROM</span>  <span class="n">Book</span>
 <span class="k">WHERE</span> <span class="n">price</span> <span class="o">&gt;</span> <span class="mi">100</span><span class="p">.</span><span class="mi">00</span>
 <span class="k">ORDER</span> <span class="k">BY</span> <span class="n">title</span><span class="p">;</span>
</pre>
</div>
<h3><span id="Subqueries" class="mw-headline">Subqueries</span></h3>
<p>Queries can be nested so that the results of one query can be used in another query via a relational operator or aggregation function. A nested query is also known as a&nbsp;<em>subquery</em>. While joins and other table operations provide computationally superior (i.e. faster) alternatives in many cases, the use of subqueries introduces a hierarchy in execution that can be useful or necessary. In the following example, the aggregation function&nbsp;<code>AVG</code>&nbsp;receives as input the result of a subquery:</p>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">SELECT</span> <span class="n">isbn</span><span class="p">,</span>
       <span class="n">title</span><span class="p">,</span>
       <span class="n">price</span>
 <span class="k">FROM</span>  <span class="n">Book</span>
 <span class="k">WHERE</span> <span class="n">price</span> <span class="o">&lt;</span> <span class="p">(</span><span class="k">SELECT</span> <span class="k">AVG</span><span class="p">(</span><span class="n">price</span><span class="p">)</span> <span class="k">FROM</span> <span class="n">Book</span><span class="p">)</span>
 <span class="k">ORDER</span> <span class="k">BY</span> <span class="n">title</span><span class="p">;</span>
</pre>
</div>
<p>A subquery can use values from the outer query, in which case it is known as a&nbsp;<a title="Correlated subquery" href="https://en.wikipedia.org/wiki/Correlated_subquery">correlated subquery</a>.</p>
<p>Since 1999 the SQL standard allows&nbsp;<code>WITH</code>&nbsp;clauses for subqueries, i.e. named subqueries, usually called&nbsp;<a class="mw-redirect" title="Common table expression" href="https://en.wikipedia.org/wiki/Common_table_expression">common table expressions</a>&nbsp;(also called&nbsp;<a class="mw-redirect" title="Subquery factoring" href="https://en.wikipedia.org/wiki/Subquery_factoring">subquery factoring</a>). CTEs can also be&nbsp;<a class="mw-redirect" title="Recursive" href="https://en.wikipedia.org/wiki/Recursive">recursive</a>&nbsp;by referring to themselves;&nbsp;<a title="Hierarchical and recursive queries in SQL" href="https://en.wikipedia.org/wiki/Hierarchical_and_recursive_queries_in_SQL">the resulting mechanism</a>&nbsp;allows tree or graph traversals (when represented as relations), and more generally&nbsp;<a class="mw-redirect" title="Fixpoint" href="https://en.wikipedia.org/wiki/Fixpoint">fixpoint</a>&nbsp;computations.</p>
<h3><span id="Derived_table" class="mw-headline">Derived table</span></h3>
<p>A&nbsp;<em>derived table</em>&nbsp;is the use of referencing an SQL subquery in a FROM clause. Essentially, the derived table is a subquery that can be selected from or joined to. The derived table functionality allows the user to reference the subquery as a table. The inline view is also referred to as an&nbsp;<em>inline view&nbsp;</em>or a&nbsp;<em>subselect</em>.</p>
<p>In the following example, the SQL statement involves a join from the initial "Book" table to the derived table "sales". This derived table captures associated book sales information using the ISBN to join to the "Book" table. As a result, the derived table provides the result set with additional columns (the number of items sold and the company that sold the books):</p>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">SELECT</span> <span class="n">b</span><span class="p">.</span><span class="n">isbn</span><span class="p">,</span> <span class="n">b</span><span class="p">.</span><span class="n">title</span><span class="p">,</span> <span class="n">b</span><span class="p">.</span><span class="n">price</span><span class="p">,</span> <span class="n">sales</span><span class="p">.</span><span class="n">items_sold</span><span class="p">,</span> <span class="n">sales</span><span class="p">.</span><span class="n">company_nm</span>
<span class="k">FROM</span> <span class="n">Book</span> <span class="n">b</span>
  <span class="k">JOIN</span> <span class="p">(</span><span class="k">SELECT</span> <span class="k">SUM</span><span class="p">(</span><span class="n">Items_Sold</span><span class="p">)</span> <span class="n">Items_Sold</span><span class="p">,</span> <span class="n">Company_Nm</span><span class="p">,</span> <span class="n">ISBN</span>
        <span class="k">FROM</span> <span class="n">Book_Sales</span>
        <span class="k">GROUP</span> <span class="k">BY</span> <span class="n">Company_Nm</span><span class="p">,</span> <span class="n">ISBN</span><span class="p">)</span> <span class="n">sales</span>
  <span class="k">ON</span> <span class="n">sales</span><span class="p">.</span><span class="n">isbn</span> <span class="o">=</span> <span class="n">b</span><span class="p">.</span><span class="n">isbn</span>
</pre>
</div>
<h3><span id="Null_or_three-valued_logic_.283VL.29"></span><span id="Null_or_three-valued_logic_(3VL)" class="mw-headline">Null or three-valued logic (3VL)</span></h3>
<div class="hatnote navigation-not-searchable">&nbsp;</div>
<p>The concept of&nbsp;<a title="Null (SQL)" href="https://en.wikipedia.org/wiki/Null_(SQL)">Null</a>&nbsp;allows SQL to deal with missing information in the relational model. The word&nbsp;<code>NULL</code>&nbsp;is a reserved keyword in SQL, used to identify the Null special marker. Comparisons with Null, for instance equality (=) in WHERE clauses, results in an Unknown truth value. In SELECT statements SQL returns only results for which the WHERE clause returns a value of True; i.e., it excludes results with values of False and also excludes those whose value is Unknown.</p>
<p>Along with True and False, the Unknown resulting from direct comparisons with Null thus brings a fragment of&nbsp;<a title="Three-valued logic" href="https://en.wikipedia.org/wiki/Three-valued_logic">three-valued logic</a>&nbsp;to SQL. The truth tables SQL uses for AND, OR, and NOT correspond to a common fragment of the Kleene and Lukasiewicz three-valued logic (which differ in their definition of implication, however SQL defines no such operation).<sup id="cite_ref-Klein_6-0" class="reference"><a href="https://en.wikipedia.org/wiki/SQL_syntax#cite_note-Klein-6">[6]</a></sup></p>
<table border="0">
<tbody>
<tr>
<td valign="top">
<table class="wikitable">
<tbody>
<tr>
<th colspan="2" rowspan="2">p AND q</th>
<th colspan="3">p</th>
</tr>
<tr>
<th>True</th>
<th>False</th>
<th>Unknown</th>
</tr>
<tr>
<th rowspan="3">q</th>
<th>True</th>
<td class="table-yes">True</td>
<td class="table-no">False</td>
<td class="unknown table-unknown">Unknown</td>
</tr>
<tr>
<th>False</th>
<td class="table-no">False</td>
<td class="table-no">False</td>
<td class="table-no">False</td>
</tr>
<tr>
<th>Unknown</th>
<td class="unknown table-unknown">Unknown</td>
<td class="table-no">False</td>
<td class="unknown table-unknown">Unknown</td>
</tr>
</tbody>
</table>
</td>
<td valign="top">
<table class="wikitable">
<tbody>
<tr>
<th colspan="2" rowspan="2">p OR q</th>
<th colspan="3">p</th>
</tr>
<tr>
<th>True</th>
<th>False</th>
<th>Unknown</th>
</tr>
<tr>
<th rowspan="3">q</th>
<th>True</th>
<td class="table-yes">True</td>
<td class="table-yes">True</td>
<td class="table-yes">True</td>
</tr>
<tr>
<th>False</th>
<td class="table-yes">True</td>
<td class="table-no">False</td>
<td class="unknown table-unknown">Unknown</td>
</tr>
<tr>
<th>Unknown</th>
<td class="table-yes">True</td>
<td class="unknown table-unknown">Unknown</td>
<td class="unknown table-unknown">Unknown</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
<table border="0">
<tbody>
<tr>
<td valign="top">
<table class="wikitable">
<tbody>
<tr>
<th colspan="2" rowspan="2">p = q</th>
<th colspan="3">p</th>
</tr>
<tr>
<th>True</th>
<th>False</th>
<th>Unknown</th>
</tr>
<tr>
<th rowspan="3">q</th>
<th>True</th>
<td class="table-yes">True</td>
<td class="table-no">False</td>
<td class="unknown table-unknown">Unknown</td>
</tr>
<tr>
<th>False</th>
<td class="table-no">False</td>
<td class="table-yes">True</td>
<td class="unknown table-unknown">Unknown</td>
</tr>
<tr>
<th>Unknown</th>
<td class="unknown table-unknown">Unknown</td>
<td class="unknown table-unknown">Unknown</td>
<td class="unknown table-unknown">Unknown</td>
</tr>
</tbody>
</table>
</td>
<td valign="top">
<table class="wikitable">
<tbody>
<tr>
<th>q</th>
<th>NOT q</th>
</tr>
<tr>
<th>True</th>
<td class="table-no">False</td>
</tr>
<tr>
<th>False</th>
<td class="table-yes">True</td>
</tr>
<tr>
<th>Unknown</th>
<td class="unknown table-unknown">Unknown</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
<p>There are however disputes about the semantic interpretation of Nulls in SQL because of its treatment outside direct comparisons. As seen in the table above, direct equality comparisons between two NULLs in SQL (e.g.&nbsp;<code>NULL = NULL</code>) return a truth value of Unknown. This is in line with the interpretation that Null does not have a value (and is not a member of any data domain) but is rather a placeholder or "mark" for missing information. However, the principle that two Nulls aren't equal to each other is effectively violated in the SQL specification for the&nbsp;<code>UNION</code>&nbsp;and&nbsp;<code>INTERSECT</code>&nbsp;operators, which do identify nulls with each other.&nbsp;Consequently, these&nbsp;<a title="Set operations (SQL)" href="https://en.wikipedia.org/wiki/Set_operations_(SQL)">set operations in SQL</a>&nbsp;may produce results not representing sure information, unlike operations involving explicit comparisons with NULL (e.g. those in a&nbsp;<code>WHERE</code>&nbsp;clause discussed above). In Codd's 1979 proposal (which was basically adopted by SQL92) this semantic inconsistency is rationalized by arguing that removal of duplicates in set operations happens "at a lower level of detail than equality testing in the evaluation of retrieval operations".&nbsp;However, computer-science professor Ron van der Meyden concluded that "The inconsistencies in the SQL standard mean that it is not possible to ascribe any intuitive logical semantics to the treatment of nulls in SQL."</p>
<p>Additionally, because SQL operators return Unknown when comparing anything with Null directly, SQL provides two Null-specific comparison predicates:&nbsp;<code>IS NULL</code>&nbsp;and&nbsp;<code>IS NOT NULL</code>&nbsp;test whether data is or is not Null.&nbsp;SQL does not explicitly support&nbsp;<a title="Universal quantification" href="https://en.wikipedia.org/wiki/Universal_quantification">universal quantification</a>, and must work it out as a negated&nbsp;<a title="Existential quantification" href="https://en.wikipedia.org/wiki/Existential_quantification">existential quantification</a>.&nbsp;There is also the "&lt;row value expression&gt; IS DISTINCT FROM &lt;row value expression&gt;" infixed comparison operator, which returns TRUE unless both operands are equal or both are NULL. Likewise, IS NOT DISTINCT FROM is defined as "NOT (&lt;row value expression&gt; IS DISTINCT FROM &lt;row value expression&gt;)".&nbsp;<a title="SQL:1999" href="https://en.wikipedia.org/wiki/SQL:1999">SQL:1999</a>&nbsp;also introduced&nbsp;<code>BOOLEAN</code>&nbsp;type variables, which according to the standard can also hold Unknown values if it is nullable. In practice, a number of systems (e.g.&nbsp;<a title="PostgreSQL" href="https://en.wikipedia.org/wiki/PostgreSQL">PostgreSQL</a>) implement the BOOLEAN Unknown as a BOOLEAN NULL, which the standard says that the NULL BOOLEAN and UNKNOWN "may be used interchangeably to mean exactly the same thing".<cite class="citation book">C. Date (2011).&nbsp;<a class="external text" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(1).pdf" rel="nofollow"><em>SQL and Relational Theory: How to Write Accurate SQL Code</em></a>. O'Reilly Media, Inc. p.&nbsp;83.&nbsp;<a title="International Standard Book Number" href="https://en.wikipedia.org/wiki/International_Standard_Book_Number">ISBN</a>&nbsp;<a title="Special:BookSources/978-1-4493-1640-2" href="https://en.wikipedia.org/wiki/Special:BookSources/978-1-4493-1640-2"><bdi>978-1-4493-1640-2</bdi></a>.</cite>&lt;/ref&gt;</p>
<h3><span id="Data_manipulation" class="mw-headline">Data manipulation</span></h3>
<p>The&nbsp;<a class="mw-redirect" title="Data Manipulation Language" href="https://en.wikipedia.org/wiki/Data_Manipulation_Language">Data Manipulation Language</a>&nbsp;(DML) is the subset of SQL used to add, update and delete data:</p>
<ul>
<li><code><a title="Insert (SQL)" href="https://en.wikipedia.org/wiki/Insert_(SQL)">INSERT</a></code>&nbsp;adds rows (formally&nbsp;<a title="Tuple" href="https://en.wikipedia.org/wiki/Tuple">tuples</a>) to an existing table, e.g.:</li>
</ul>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">INSERT</span> <span class="k">INTO</span> <span class="n">example</span>
 <span class="p">(</span><span class="n">column1</span><span class="p">,</span> <span class="n">column2</span><span class="p">,</span> <span class="n">column3</span><span class="p">)</span>
 <span class="k">VALUES</span>
 <span class="p">(</span><span class="s1">'test'</span><span class="p">,</span> <span class="s1">'N'</span><span class="p">,</span> <span class="k">NULL</span><span class="p">);</span>
</pre>
</div>
<ul>
<li><code><a title="Update (SQL)" href="https://en.wikipedia.org/wiki/Update_(SQL)">UPDATE</a></code>&nbsp;modifies a set of existing table rows, e.g.:</li>
</ul>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">UPDATE</span> <span class="n">example</span>
 <span class="k">SET</span> <span class="n">column1</span> <span class="o">=</span> <span class="s1">'updated value'</span>
 <span class="k">WHERE</span> <span class="n">column2</span> <span class="o">=</span> <span class="s1">'N'</span><span class="p">;</span>
</pre>
</div>
<ul>
<li><code><a title="Delete (SQL)" href="https://en.wikipedia.org/wiki/Delete_(SQL)">DELETE</a></code>&nbsp;removes existing rows from a table, e.g.:</li>
</ul>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">DELETE</span> <span class="k">FROM</span> <span class="n">example</span>
 <span class="k">WHERE</span> <span class="n">column2</span> <span class="o">=</span> <span class="s1">'N'</span><span class="p">;</span>
</pre>
</div>
<ul>
<li><code><a title="Merge (SQL)" href="https://en.wikipedia.org/wiki/Merge_(SQL)">MERGE</a></code>&nbsp;is used to combine the data of multiple tables. It combines the&nbsp;<code>INSERT</code>&nbsp;and&nbsp;<code>UPDATE</code>&nbsp;elements. It is defined in the SQL:2003 standard; prior to that, some databases provided similar functionality via different syntax, sometimes called "<a class="mw-redirect" title="Upsert" href="https://en.wikipedia.org/wiki/Upsert">upsert</a>".</li>
</ul>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre> <span class="n">MERGE</span> <span class="k">INTO</span> <span class="k">table_name</span> <span class="k">USING</span> <span class="n">table_reference</span> <span class="k">ON</span> <span class="p">(</span><span class="n">condition</span><span class="p">)</span>
 <span class="k">WHEN</span> <span class="n">MATCHED</span> <span class="k">THEN</span>
 <span class="k">UPDATE</span> <span class="k">SET</span> <span class="n">column1</span> <span class="o">=</span> <span class="n">value1</span> <span class="p">[,</span> <span class="n">column2</span> <span class="o">=</span> <span class="n">value2</span> <span class="p">...]</span>
 <span class="k">WHEN</span> <span class="k">NOT</span> <span class="n">MATCHED</span> <span class="k">THEN</span>
 <span class="k">INSERT</span> <span class="p">(</span><span class="n">column1</span> <span class="p">[,</span> <span class="n">column2</span> <span class="p">...])</span> <span class="k">VALUES</span> <span class="p">(</span><span class="n">value1</span> <span class="p">[,</span> <span class="n">value2</span> <span class="p">...])</span>
</pre>
</div>
<h3><span id="Transaction_controls" class="mw-headline">Transaction controls</span></h3>
<p>Transactions, if available, wrap DML operations:</p>
<ul>
<li><code>START TRANSACTION</code>&nbsp;(or&nbsp;<code>BEGIN WORK</code>, or&nbsp;<code>BEGIN TRANSACTION</code>, depending on SQL dialect) marks the start of a&nbsp;<a title="Database transaction" href="https://en.wikipedia.org/wiki/Database_transaction">database transaction</a>, which either completes entirely or not at all.</li>
<li><code>SAVE TRANSACTION</code>&nbsp;(or&nbsp;<code>SAVEPOINT</code>) saves the state of the database at the current point in transaction</li>
</ul>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">CREATE</span> <span class="k">TABLE</span> <span class="n">tbl_1</span><span class="p">(</span><span class="n">id</span> <span class="nb">int</span><span class="p">);</span>
 <span class="k">INSERT</span> <span class="k">INTO</span> <span class="n">tbl_1</span><span class="p">(</span><span class="n">id</span><span class="p">)</span> <span class="k">VALUES</span><span class="p">(</span><span class="mf">1</span><span class="p">);</span>
 <span class="k">INSERT</span> <span class="k">INTO</span> <span class="n">tbl_1</span><span class="p">(</span><span class="n">id</span><span class="p">)</span> <span class="k">VALUES</span><span class="p">(</span><span class="mf">2</span><span class="p">);</span>
<span class="k">COMMIT</span><span class="p">;</span>
 <span class="k">UPDATE</span> <span class="n">tbl_1</span> <span class="k">SET</span> <span class="n">id</span><span class="o">=</span><span class="mf">200</span> <span class="k">WHERE</span> <span class="n">id</span><span class="o">=</span><span class="mf">1</span><span class="p">;</span>
<span class="k">SAVEPOINT</span> <span class="n">id_1upd</span><span class="p">;</span>
 <span class="k">UPDATE</span> <span class="n">tbl_1</span> <span class="k">SET</span> <span class="n">id</span><span class="o">=</span><span class="mf">1000</span> <span class="k">WHERE</span> <span class="n">id</span><span class="o">=</span><span class="mf">2</span><span class="p">;</span>
<span class="k">ROLLBACK</span> <span class="k">to</span> <span class="n">id_1upd</span><span class="p">;</span>
 <span class="k">SELECT</span> <span class="n">id</span> <span class="k">from</span> <span class="n">tbl_1</span><span class="p">;</span>
</pre>
</div>
<ul>
<li><code><a class="mw-redirect" title="Commit (SQL)" href="https://en.wikipedia.org/wiki/Commit_(SQL)">COMMIT</a></code>&nbsp;makes all data changes in a transaction permanent.</li>
<li><code><a class="mw-redirect" title="Rollback (SQL)" href="https://en.wikipedia.org/wiki/Rollback_(SQL)">ROLLBACK</a></code>&nbsp;discards all data changes since the last&nbsp;<code>COMMIT</code>&nbsp;or&nbsp;<code>ROLLBACK</code>, leaving the data as it was prior to those changes. Once the&nbsp;<code>COMMIT</code>&nbsp;statement completes, the transaction's changes cannot be rolled back.</li>
</ul>
<p><code>COMMIT</code>&nbsp;and&nbsp;<code>ROLLBACK</code>&nbsp;terminate the current transaction and release data locks. In the absence of a&nbsp;<code>START TRANSACTION</code>&nbsp;or similar statement, the semantics of SQL are implementation-dependent. The following example shows a classic transfer of funds transaction, where money is removed from one account and added to another. If either the removal or the addition fails, the entire transaction is rolled back.</p>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">START</span> <span class="k">TRANSACTION</span><span class="p">;</span>
 <span class="k">UPDATE</span> <span class="n">Account</span> <span class="k">SET</span> <span class="n">amount</span><span class="o">=</span><span class="n">amount</span><span class="o">-</span><span class="mf">200</span> <span class="k">WHERE</span> <span class="n">account_number</span><span class="o">=</span><span class="mf">1234</span><span class="p">;</span>
 <span class="k">UPDATE</span> <span class="n">Account</span> <span class="k">SET</span> <span class="n">amount</span><span class="o">=</span><span class="n">amount</span><span class="o">+</span><span class="mf">200</span> <span class="k">WHERE</span> <span class="n">account_number</span><span class="o">=</span><span class="mf">2345</span><span class="p">;</span>

<span class="k">IF</span> <span class="n">ERRORS</span><span class="o">=</span><span class="mf">0</span> <span class="k">COMMIT</span><span class="p">;</span>
<span class="k">IF</span> <span class="n">ERRORS</span><span class="o">&lt;&gt;</span><span class="mf">0</span> <span class="k">ROLLBACK</span><span class="p">;</span>
</pre>
</div>
<h3><span id="Data_definition" class="mw-headline">Data definition</span></h3>
<p>The&nbsp;<a class="mw-redirect" title="Data Definition Language" href="https://en.wikipedia.org/wiki/Data_Definition_Language">Data Definition Language</a>&nbsp;(DDL) manages table and index structure. The most basic items of DDL are the&nbsp;<code>CREATE</code>,&nbsp;<code>ALTER</code>,&nbsp;<code>RENAME</code>,&nbsp;<code>DROP</code>&nbsp;and&nbsp;<code>TRUNCATE</code>&nbsp;statements:</p>
<ul>
<li><code><a class="mw-redirect" title="Create (SQL)" href="https://en.wikipedia.org/wiki/Create_(SQL)">CREATE</a></code>&nbsp;creates an object (a table, for example) in the database, e.g.:</li>
</ul>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">CREATE</span> <span class="k">TABLE</span> <span class="n">example</span><span class="p">(</span>
 <span class="n">column1</span> <span class="nb">INTEGER</span><span class="p">,</span>
 <span class="n">column2</span> <span class="nb">VARCHAR</span><span class="p">(</span><span class="mi">50</span><span class="p">),</span>
 <span class="n">column3</span> <span class="nb">DATE</span> <span class="k">NOT</span> <span class="k">NULL</span><span class="p">,</span>
 <span class="k">PRIMARY</span> <span class="k">KEY</span> <span class="p">(</span><span class="n">column1</span><span class="p">,</span> <span class="n">column2</span><span class="p">)</span>
<span class="p">);</span>
</pre>
</div>
<ul>
<li><code><a class="mw-redirect" title="Alter (SQL)" href="https://en.wikipedia.org/wiki/Alter_(SQL)">ALTER</a></code>&nbsp;modifies the structure of an existing object in various ways, for example, adding a column to an existing table or a constraint, e.g.:</li>
</ul>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">ALTER</span> <span class="k">TABLE</span> <span class="n">example</span> <span class="k">ADD</span> <span class="n">column4</span> <span class="nb">INTEGER</span> <span class="k">DEFAULT</span> <span class="mi">25</span> <span class="k">NOT</span> <span class="k">NULL</span><span class="p">;</span>
</pre>
</div>
<ul>
<li><code><a title="Truncate (SQL)" href="https://en.wikipedia.org/wiki/Truncate_(SQL)">TRUNCATE</a></code>&nbsp;deletes all data from a table in a very fast way, deleting the data inside the table and not the table itself. It usually implies a subsequent COMMIT operation, i.e., it cannot be rolled back (data is not written to the logs for rollback later, unlike DELETE).</li>
</ul>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">TRUNCATE</span> <span class="k">TABLE</span> <span class="n">example</span><span class="p">;</span>
</pre>
</div>
<ul>
<li><code><a class="mw-redirect" title="Drop (SQL)" href="https://en.wikipedia.org/wiki/Drop_(SQL)">DROP</a></code>&nbsp;deletes an object in the database, usually irretrievably, i.e., it cannot be rolled back, e.g.:</li>
</ul>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">DROP</span> <span class="k">TABLE</span> <span class="n">example</span><span class="p">;</span>
</pre>
</div>
<h3><span id="Data_types" class="mw-headline">Data types</span></h3>
<p>Each column in an SQL table declares the type(s) that column may contain. ANSI SQL includes the following data types.</p>
<dl>
<dt>Character strings and national character strings</dt>
</dl>
<ul>
<li><code>CHARACTER(<var>n</var>)</code>&nbsp;(or&nbsp;<code>CHAR(<var>n</var>)</code>): fixed-width&nbsp;<var>n</var>-character string, padded with spaces as needed</li>
<li><code>CHARACTER VARYING(<var>n</var>)</code>&nbsp;(or&nbsp;<code>VARCHAR(<var>n</var>)</code>): variable-width string with a maximum size of&nbsp;<var>n</var>&nbsp;characters</li>
<li><code>CHARACTER LARGE OBJECT(<var>n</var>&nbsp;[ K | M | G | T ])</code>&nbsp;(or&nbsp;<code>CLOB(<var>n</var>&nbsp;[ K | M | G | T ])</code>): character large object with a maximum size of&nbsp;<var>n [ K | M | G | T ]</var>&nbsp;characters</li>
<li><code>NATIONAL CHARACTER(<var>n</var>)</code>&nbsp;(or&nbsp;<code>NCHAR(<var>n</var>)</code>): fixed width string supporting an international character set</li>
<li><code>NATIONAL CHARACTER VARYING(<var>n</var>)</code>&nbsp;(or&nbsp;<code>NVARCHAR(<var>n</var>)</code>): variable-width&nbsp;<code>NCHAR</code>&nbsp;string</li>
<li><code>NATIONAL CHARACTER LARGE OBJECT(<var>n</var>&nbsp;[ K | M | G | T ])</code>&nbsp;(or&nbsp;<code>NCLOB(<var>n</var>&nbsp;[ K | M | G | T ])</code>): national character large object with a maximum size of&nbsp;<var>n [ K | M | G | T ]</var>&nbsp;characters</li>
</ul>
<p>For the&nbsp;<code>CHARACTER LARGE OBJECT</code>&nbsp;and&nbsp;<code>NATIONAL CHARACTER LARGE OBJECT</code>&nbsp;data types, the multipliers&nbsp;<code>K</code>&nbsp;(1 024),&nbsp;<code>M</code>&nbsp;(1 048 576),&nbsp;<code>G</code>&nbsp;(1 073 741 824) and&nbsp;<code>T</code>&nbsp;(1 099 511 627 776) can be optionally used when specifying the length.</p>
<dl>
<dt>Binary</dt>
</dl>
<ul>
<li><code>BINARY(<var>n</var>)</code>: Fixed length binary string, maximum length&nbsp;<var>n</var>.</li>
<li><code>BINARY VARYING(<var>n</var>)</code>&nbsp;(or&nbsp;<code>VARBINARY(<var>n</var>)</code>): Variable length binary string, maximum length&nbsp;<var>n</var>.</li>
<li><code>BINARY LARGE OBJECT(<var>n</var>&nbsp;[ K | M | G | T ])</code>&nbsp;(or&nbsp;<code>BLOB(<var>n</var>&nbsp;[ K | M | G | T ])</code>): binary large object with a maximum length&nbsp;<var>n [ K | M | G | T ]</var>.</li>
</ul>
<p>For the&nbsp;<code>BINARY LARGE OBJECT</code>&nbsp;data type, the multipliers&nbsp;<code>K</code>&nbsp;(1 024),&nbsp;<code>M</code>&nbsp;(1 048 576),&nbsp;<code>G</code>&nbsp;(1 073 741 824) and&nbsp;<code>T</code>&nbsp;(1 099 511 627 776) can be optionally used when specifying the length.</p>
<dl>
<dt>Boolean</dt>
</dl>
<ul>
<li><code>BOOLEAN</code></li>
</ul>
<p>The&nbsp;<code>BOOLEAN</code>&nbsp;data type can store the values&nbsp;<code>TRUE</code>&nbsp;and&nbsp;<code>FALSE</code>.</p>
<dl>
<dt>Numerical</dt>
</dl>
<ul>
<li><code>INTEGER</code>&nbsp;(or&nbsp;<code>INT</code>),&nbsp;<code>SMALLINT</code>&nbsp;and&nbsp;<code>BIGINT</code></li>
<li><code>FLOAT</code>,&nbsp;<code>REAL</code>&nbsp;and&nbsp;<code>DOUBLE PRECISION</code></li>
<li><code>NUMERIC(<var>precision</var>,&nbsp;<var>scale</var>)</code>&nbsp;or&nbsp;<code>DECIMAL(<var>precision</var>,&nbsp;<var>scale</var>)</code></li>
<li><code>DECFLOAT(<var>precision</var></code>)</li>
</ul>
<p>For example, the number 123.45 has a precision of 5 and a scale of 2. The&nbsp;<var>precision</var>&nbsp;is a positive integer that determines the number of significant digits in a particular radix (binary or decimal). The&nbsp;<var>scale</var>&nbsp;is a non-negative integer. A scale of 0 indicates that the number is an integer. For a decimal number with scale S, the exact numeric value is the integer value of the significant digits divided by 10<sup>S</sup>.</p>
<p>SQL provides the functions&nbsp;<code>CEILING</code>&nbsp;and&nbsp;<code>FLOOR</code>&nbsp;to round numerical values. (Popular vendor specific functions are&nbsp;<code>TRUNC</code>&nbsp;(Informix, DB2, PostgreSQL, Oracle and MySQL) and&nbsp;<code>ROUND</code>&nbsp;(Informix, SQLite, Sybase, Oracle, PostgreSQL, Microsoft SQL Server and Mimer SQL.))</p>
<dl>
<dt>Temporal (datetime)</dt>
</dl>
<ul>
<li><code>DATE</code>: for date values (e.g.&nbsp;<code>2011-05-03</code>)</li>
<li><code>TIME</code>: for time values (e.g.&nbsp;<code>15:51:36</code>).</li>
<li><code>TIME WITH TIME ZONE</code>: the same as&nbsp;<code>TIME</code>, but including details about the time zone in question.</li>
<li><code>TIMESTAMP</code>: This is a&nbsp;<code>DATE</code>&nbsp;and a&nbsp;<code>TIME</code>&nbsp;put together in one variable (e.g.&nbsp;<code>2011-05-03 15:51:36.123456</code>).</li>
<li><code>TIMESTAMP WITH TIME ZONE</code>: the same as&nbsp;<code>TIMESTAMP</code>, but including details about the time zone in question.</li>
</ul>
<p>The SQL function&nbsp;<code>EXTRACT</code>&nbsp;can be used for extracting a single field (seconds, for instance) of a datetime or interval value. The current system date / time of the database server can be called by using functions like&nbsp;<code>CURRENT_DATE</code>,&nbsp;<code>CURRENT_TIMESTAMP</code>,&nbsp;<code>LOCALTIME</code>, or&nbsp;<code>LOCALTIMESTAMP</code>. (Popular vendor specific functions are&nbsp;<code>TO_DATE</code>,&nbsp;<code>TO_TIME</code>,&nbsp;<code>TO_TIMESTAMP</code>,&nbsp;<code>YEAR</code>,&nbsp;<code>MONTH</code>,&nbsp;<code>DAY</code>,&nbsp;<code>HOUR</code>,&nbsp;<code>MINUTE</code>,&nbsp;<code>SECOND</code>,&nbsp;<code>DAYOFYEAR</code>,&nbsp;<code>DAYOFMONTH</code>&nbsp;and&nbsp;<code>DAYOFWEEK</code>.)</p>
<dl>
<dt>Interval (datetime)</dt>
</dl>
<ul>
<li><code>YEAR(<var>precision</var>)</code>: a number of years</li>
<li><code>YEAR(<var>precision</var>) TO MONTH</code>: a number of years and months</li>
<li><code>MONTH(<var>precision</var>)</code>: a number of months</li>
<li><code>DAY(<var>precision</var>)</code>: a number of days</li>
<li><code>DAY(<var>precision</var>) TO HOUR</code>: a number of days and hours</li>
<li><code>DAY(<var>precision</var>) TO MINUTE</code>: a number of days, hours and minutes</li>
<li><code>DAY(<var>precision</var>) TO SECOND(<var>scale</var>)</code>: a number of days, hours, minutes and seconds</li>
<li><code>HOUR(<var>precision</var>)</code>: a number of hours</li>
<li><code>HOUR(<var>precision</var>) TO MINUTE</code>: a number of hours and minutes</li>
<li><code>HOUR(<var>precision</var>) TO SECOND(<var>scale</var>)</code>: a number of hours, minutes and seconds</li>
<li><code>MINUTE(<var>precision</var>)</code>: a number of minutes</li>
<li><code>MINUTE(<var>precision</var>) TO SECOND(<var>scale</var>)</code>: a number of minutes and seconds</li>
</ul>
<h3><span id="Data_control" class="mw-headline">Data control</span></h3>
<p>The&nbsp;<a class="mw-redirect" title="Data Control Language" href="https://en.wikipedia.org/wiki/Data_Control_Language">Data Control Language</a>&nbsp;(DCL) authorizes users to access and manipulate data. Its two main statements are:</p>
<ul>
<li><code>GRANT</code>&nbsp;authorizes one or more users to perform an operation or a set of operations on an object.</li>
<li><code>REVOKE</code>&nbsp;eliminates a grant, which may be the default grant.</li>
</ul>
<p>Example:</p>
<div class="mw-highlight mw-content-ltr" dir="ltr">
<pre><span class="k">GRANT</span> <span class="k">SELECT</span><span class="p">,</span> <span class="k">UPDATE</span>
 <span class="k">ON</span> <span class="n">example</span>
 <span class="k">TO</span> <span class="n">some_user</span><span class="p">,</span> <span class="n">another_user</span><span class="p">;</span>

<span class="k">REVOKE</span> <span class="k">SELECT</span><span class="p">,</span> <span class="k">UPDATE</span>
 <span class="k">ON</span> <span class="n">example</span>
 <span class="k">FROM</span> <span class="n">some_user</span><span class="p">,</span> <span class="n">another_user</span><span class="p">;</span>
</pre>
</div>

</br>

<h2><span id="Procedural_extensions" class="mw-headline">Procedural extensions</span></h2>
<p>SQL is designed for a specific purpose: to query&nbsp;<a title="Data" href="https://en.wikipedia.org/wiki/Data">data</a>&nbsp;contained in a&nbsp;<a title="Relational database" href="https://en.wikipedia.org/wiki/Relational_database">relational database</a>. SQL is a&nbsp;<a class="mw-redirect" title="Set (computer science)" href="https://en.wikipedia.org/wiki/Set_(computer_science)">set</a>-based,&nbsp;<a class="mw-redirect" title="Declarative programming language" href="https://en.wikipedia.org/wiki/Declarative_programming_language">declarative programming language</a>, not an&nbsp;<a class="mw-redirect" title="Imperative programming language" href="https://en.wikipedia.org/wiki/Imperative_programming_language">imperative programming language</a>&nbsp;like&nbsp;<a title="C (programming language)" href="https://en.wikipedia.org/wiki/C_(programming_language)">C</a>&nbsp;or&nbsp;<a title="BASIC" href="https://en.wikipedia.org/wiki/BASIC">BASIC</a>. However, extensions to Standard SQL add&nbsp;<a class="mw-redirect" title="Procedural programming language" href="https://en.wikipedia.org/wiki/Procedural_programming_language">procedural programming language</a>&nbsp;functionality, such as control-of-flow constructs. These include:</p>
<table class="wikitable">
<tbody>
<tr>
<th>Source</th>
<th>Abbreviation</th>
<th>Full name</th>
</tr>
<tr>
<td>ANSI/ISO Standard</td>
<td><a title="SQL/PSM" href="https://en.wikipedia.org/wiki/SQL/PSM">SQL/PSM</a></td>
<td>SQL/Persistent Stored Modules</td>
</tr>
<tr>
<td><a class="mw-redirect" title="Interbase" href="https://en.wikipedia.org/wiki/Interbase">Interbase</a>&nbsp;/&nbsp;<a title="Firebird (database server)" href="https://en.wikipedia.org/wiki/Firebird_(database_server)">Firebird</a></td>
<td><a class="mw-redirect" title="Procedural SQL" href="https://en.wikipedia.org/wiki/Procedural_SQL">PSQL</a></td>
<td>Procedural SQL</td>
</tr>
<tr>
<td><a class="mw-redirect" title="IBM DB2" href="https://en.wikipedia.org/wiki/IBM_DB2">IBM DB2</a></td>
<td><a title="SQL PL" href="https://en.wikipedia.org/wiki/SQL_PL">SQL PL</a></td>
<td>SQL Procedural Language (implements SQL/PSM)</td>
</tr>
<tr>
<td><a title="IBM Informix" href="https://en.wikipedia.org/wiki/IBM_Informix">IBM Informix</a></td>
<td>SPL</td>
<td>Stored Procedural Language</td>
</tr>
<tr>
<td>IBM&nbsp;<a title="Netezza" href="https://en.wikipedia.org/wiki/Netezza">Netezza</a></td>
<td>NZPLSQL</td>
<td>(based on Postgres PL/pgSQL)</td>
</tr>
<tr>
<td>Invantive</td>
<td>PSQL</td>
<td>Invantive Procedural SQL (implements&nbsp;<a title="SQL/PSM" href="https://en.wikipedia.org/wiki/SQL/PSM">SQL/PSM</a>&nbsp;and&nbsp;<a title="PL/SQL" href="https://en.wikipedia.org/wiki/PL/SQL">PL/SQL</a>)</td>
</tr>
<tr>
<td><a title="MariaDB" href="https://en.wikipedia.org/wiki/MariaDB">MariaDB</a></td>
<td><a title="SQL/PSM" href="https://en.wikipedia.org/wiki/SQL/PSM">SQL/PSM</a>,&nbsp;<a title="PL/SQL" href="https://en.wikipedia.org/wiki/PL/SQL">PL/SQL</a></td>
<td>SQL/Persistent Stored Module (implements SQL/PSM), Procedural Language/SQL (based on&nbsp;<a title="Ada (programming language)" href="https://en.wikipedia.org/wiki/Ada_(programming_language)">Ada</a>)</td>
</tr>
<tr>
<td><a title="Microsoft" href="https://en.wikipedia.org/wiki/Microsoft">Microsoft</a>&nbsp;/&nbsp;<a title="Sybase" href="https://en.wikipedia.org/wiki/Sybase">Sybase</a></td>
<td><a title="Transact-SQL" href="https://en.wikipedia.org/wiki/Transact-SQL">T-SQL</a></td>
<td>Transact-SQL</td>
</tr>
<tr>
<td><a title="Mimer SQL" href="https://en.wikipedia.org/wiki/Mimer_SQL">Mimer SQL</a></td>
<td><a title="SQL/PSM" href="https://en.wikipedia.org/wiki/SQL/PSM">SQL/PSM</a></td>
<td>SQL/Persistent Stored Module (implements SQL/PSM)</td>
</tr>
<tr>
<td><a title="MySQL" href="https://en.wikipedia.org/wiki/MySQL">MySQL</a></td>
<td><a title="SQL/PSM" href="https://en.wikipedia.org/wiki/SQL/PSM">SQL/PSM</a></td>
<td>SQL/Persistent Stored Module (implements SQL/PSM)</td>
</tr>
<tr>
<td><a title="MonetDB" href="https://en.wikipedia.org/wiki/MonetDB">MonetDB</a></td>
<td><a title="SQL/PSM" href="https://en.wikipedia.org/wiki/SQL/PSM">SQL/PSM</a></td>
<td>SQL/Persistent Stored Module (implements SQL/PSM)</td>
</tr>
<tr>
<td><a title="NuoDB" href="https://en.wikipedia.org/wiki/NuoDB">NuoDB</a></td>
<td>SSP</td>
<td>Starkey Stored Procedures</td>
</tr>
<tr>
<td><a title="Oracle Database" href="https://en.wikipedia.org/wiki/Oracle_Database">Oracle</a></td>
<td><a title="PL/SQL" href="https://en.wikipedia.org/wiki/PL/SQL">PL/SQL</a></td>
<td>Procedural Language/SQL (based on&nbsp;<a title="Ada (programming language)" href="https://en.wikipedia.org/wiki/Ada_(programming_language)">Ada</a>)</td>
</tr>
<tr>
<td><a title="PostgreSQL" href="https://en.wikipedia.org/wiki/PostgreSQL">PostgreSQL</a></td>
<td><a title="PL/pgSQL" href="https://en.wikipedia.org/wiki/PL/pgSQL">PL/pgSQL</a></td>
<td>Procedural Language/PostgreSQL Structured Query Language (implements SQL/PSM)</td>
</tr>
<tr>
<td><a title="SAP SE" href="https://en.wikipedia.org/wiki/SAP_SE">SAP R/3</a></td>
<td><a title="ABAP" href="https://en.wikipedia.org/wiki/ABAP">ABAP</a></td>
<td>Advanced Business Application Programming</td>
</tr>
<tr>
<td><a title="SAP HANA" href="https://en.wikipedia.org/wiki/SAP_HANA">SAP HANA</a></td>
<td>SQLScript</td>
<td>SQLScript</td>
</tr>
<tr>
<td><a title="Sybase" href="https://en.wikipedia.org/wiki/Sybase">Sybase</a></td>
<td>Watcom-SQL</td>
<td>SQL Anywhere Watcom-SQL Dialect</td>
</tr>
<tr>
<td><a title="Teradata" href="https://en.wikipedia.org/wiki/Teradata">Teradata</a></td>
<td>SPL</td>
<td>Stored Procedural Language</td>
</tr>
</tbody>
</table>
<p>In addition to the standard SQL/PSM extensions and proprietary SQL extensions, procedural and&nbsp;<a class="mw-redirect" title="Object-oriented programming language" href="https://en.wikipedia.org/wiki/Object-oriented_programming_language">object-oriented</a>&nbsp;programmability is available on many SQL platforms via DBMS integration with other languages. The SQL standard defines&nbsp;<a title="SQL/JRT" href="https://en.wikipedia.org/wiki/SQL/JRT">SQL/JRT</a>&nbsp;extensions (SQL Routines and Types for the Java Programming Language) to support&nbsp;<a title="Java (programming language)" href="https://en.wikipedia.org/wiki/Java_(programming_language)">Java</a>&nbsp;code in SQL databases.&nbsp;<a class="mw-redirect" title="Microsoft SQL Server 2005" href="https://en.wikipedia.org/wiki/Microsoft_SQL_Server_2005">Microsoft SQL Server 2005</a>&nbsp;uses the&nbsp;<a class="mw-redirect" title="SQLCLR" href="https://en.wikipedia.org/wiki/SQLCLR">SQLCLR</a>&nbsp;(SQL Server Common Language Runtime) to host managed&nbsp;<a class="mw-redirect" title="Microsoft .NET" href="https://en.wikipedia.org/wiki/Microsoft_.NET">.NET</a>&nbsp;assemblies in the database, while prior versions of SQL Server were restricted to unmanaged extended stored procedures primarily written in C.&nbsp;<a title="PostgreSQL" href="https://en.wikipedia.org/wiki/PostgreSQL">PostgreSQL</a>&nbsp;lets users write functions in a wide variety of languages&mdash;including&nbsp;<a title="Perl" href="https://en.wikipedia.org/wiki/Perl">Perl</a>,&nbsp;<a title="Python (programming language)" href="https://en.wikipedia.org/wiki/Python_(programming_language)">Python</a>,&nbsp;<a title="Tcl" href="https://en.wikipedia.org/wiki/Tcl">Tcl</a>,&nbsp;<a title="JavaScript" href="https://en.wikipedia.org/wiki/JavaScript">JavaScript</a>&nbsp;(PL/V8) and C.</p>
<h2><span id="Interoperability_and_standardization" class="mw-headline">Interoperability and standardization</span></h2>
<p>SQL implementations are incompatible between vendors and do not necessarily completely follow standards. In particular date and time syntax, string concatenation,&nbsp;<code>NULL</code>s, and comparison&nbsp;<a title="Case sensitivity" href="https://en.wikipedia.org/wiki/Case_sensitivity">case sensitivity</a>&nbsp;vary from vendor to vendor. Particular exceptions are&nbsp;<a title="PostgreSQL" href="https://en.wikipedia.org/wiki/PostgreSQL">PostgreSQL</a>&nbsp;and&nbsp;<a title="Mimer SQL" href="https://en.wikipedia.org/wiki/Mimer_SQL">Mimer SQL</a>&nbsp;which strive for standards compliance, though PostgreSQL does not adhere to the standard in how folding of unquoted names is done. The folding of unquoted names to lower case in PostgreSQL is incompatible with the SQL standard,&nbsp;which says that unquoted names should be folded to upper case.&nbsp;Thus,&nbsp;<code>Foo</code>&nbsp;should be equivalent to&nbsp;<code>FOO</code>&nbsp;not&nbsp;<code>foo</code>&nbsp;according to the standard.</p>
<p>Popular implementations of SQL commonly omit support for basic features of Standard SQL, such as the&nbsp;<code>DATE</code>&nbsp;or&nbsp;<code>TIME</code>&nbsp;data types. The most obvious such examples, and incidentally the most popular commercial and proprietary SQL DBMSs, are Oracle (whose&nbsp;<code>DATE</code>&nbsp;behaves as&nbsp;<code>DATETIME</code>,&nbsp;and lacks a&nbsp;<code>TIME</code>&nbsp;type)&nbsp;and MS SQL Server (before the 2008 version). As a result, SQL code can rarely be ported between database systems without modifications.</p>
<p>There are several reasons for this lack of portability between database systems:</p>
<ul>
<li>The complexity and size of the SQL standard means that most implementors do not support the entire standard.</li>
<li>The standard does not specify database behavior in several important areas (e.g.&nbsp;<a class="mw-redirect" title="Index (database)" href="https://en.wikipedia.org/wiki/Index_(database)">indexes</a>, file storage...), leaving implementations to decide how to behave.</li>
<li>The SQL standard precisely specifies the syntax that a conforming database system must implement. However, the standard's specification of the semantics of language constructs is less well-defined, leading to ambiguity.</li>
<li>Many database vendors have large existing customer bases; where the newer version of the SQL standard conflicts with the prior behavior of the vendor's database, the vendor may be unwilling to break&nbsp;<a title="Backward compatibility" href="https://en.wikipedia.org/wiki/Backward_compatibility">backward compatibility</a>.</li>
<li>There is little commercial incentive for vendors to make it easier for users to change database suppliers.</li>
<li>Users evaluating database software tend to place other factors such as performance higher in their priorities than standards conformance.</li>
</ul>
<p>SQL was adopted as a standard by the&nbsp;<a title="American National Standards Institute" href="https://en.wikipedia.org/wiki/American_National_Standards_Institute">American National Standards Institute</a>&nbsp;(ANSI) in 1986 as SQL-86&nbsp;and the&nbsp;<a title="International Organization for Standardization" href="https://en.wikipedia.org/wiki/International_Organization_for_Standardization">International Organization for Standardization</a>&nbsp;(ISO) in 1987.&nbsp;It is maintained by&nbsp;<a title="ISO/IEC JTC 1/SC 32" href="https://en.wikipedia.org/wiki/ISO/IEC_JTC_1/SC_32"><em>ISO/IEC JTC 1, Information technology, Subcommittee SC 32, Data management and interchange</em></a>. The standard is commonly denoted by the pattern:&nbsp;<em>ISO/IEC 9075-n:yyyy Part n: title</em>, or, as a shortcut,&nbsp;<em>ISO/IEC 9075</em>.</p>
<p><em>ISO/IEC 9075</em>&nbsp;is complemented by&nbsp;<em>ISO/IEC 13249: SQL Multimedia and Application Packages</em>&nbsp;(SQL/MM), which defines SQL based interfaces and packages to widely spread applications like video, audio and&nbsp;<a class="mw-redirect" title="Georeference" href="https://en.wikipedia.org/wiki/Georeference">spatial data</a>.</p>
<p>Until 1996, the&nbsp;<a title="National Institute of Standards and Technology" href="https://en.wikipedia.org/wiki/National_Institute_of_Standards_and_Technology">National Institute of Standards and Technology</a>&nbsp;(NIST) data management standards program certified SQL DBMS compliance with the SQL standard. Vendors now self-certify the compliance of their products.</p>
<p>The original standard declared that the official pronunciation for "SQL" was an&nbsp;<a class="mw-redirect" title="Initialism" href="https://en.wikipedia.org/wiki/Initialism">initialism</a>:&nbsp;<span class="rt-commentedText nowrap"><span class="IPA nopopups noexcerpt"><a title="Help:IPA/English" href="https://en.wikipedia.org/wiki/Help:IPA/English">/<span title="/ˌ/: secondary stress follows">ˌ</span><span title="/ɛ/: 'e' in 'dress'">ɛ</span><span title="'s' in 'sigh'">s</span><span title="/ˌ/: secondary stress follows">ˌ</span><span title="'k' in 'kind'">k</span><span title="/juː/: 'u' in 'cute'">juː</span><span title="/ˈ/: primary stress follows">ˈ</span><span title="/ɛ/: 'e' in 'dress'">ɛ</span><span title="'l' in 'lie'">l</span>/</a></span></span>&nbsp;("ess cue el").&nbsp;Regardless, many English-speaking database professionals (including&nbsp;<a class="mw-redirect" title="Donald Chamberlin" href="https://en.wikipedia.org/wiki/Donald_Chamberlin">Donald Chamberlin</a>&nbsp;himself) use the&nbsp;<a title="Acronym" href="https://en.wikipedia.org/wiki/Acronym">acronym</a>-like pronunciation of&nbsp;<span class="rt-commentedText nowrap"><span class="IPA nopopups noexcerpt"><a title="Help:IPA/English" href="https://en.wikipedia.org/wiki/Help:IPA/English">/<span title="/ˈ/: primary stress follows">ˈ</span><span title="'s' in 'sigh'">s</span><span title="/iː/: 'ee' in 'fleece'">iː</span><span title="'k' in 'kind'">k</span><span title="'w' in 'wind'">w</span><span title="/əl/: 'le' in 'bottle'">əl</span>/</a></span></span>&nbsp;("sequel"),&nbsp;mirroring the language's pre-release development name of "SEQUEL".&nbsp;The SQL standard has gone through a number of revisions:</p>
<table class="wikitable">
<tbody>
<tr>
<th>Year</th>
<th>Name</th>
<th>Alias</th>
<th>Comments</th>
</tr>
<tr>
<td>1986</td>
<td>SQL-86</td>
<td>SQL-87</td>
<td>First formalized by ANSI.</td>
</tr>
<tr>
<td>1989</td>
<td>SQL-89</td>
<td><a class="mw-redirect" title="Federal Information Processing Standard" href="https://en.wikipedia.org/wiki/Federal_Information_Processing_Standard">FIPS</a>&nbsp;127-1</td>
<td>Minor revision that added integrity constraints, adopted as FIPS 127-1.</td>
</tr>
<tr>
<td>1992</td>
<td><a title="SQL-92" href="https://en.wikipedia.org/wiki/SQL-92">SQL-92</a></td>
<td>SQL2, FIPS 127-2</td>
<td>Major revision (ISO 9075),&nbsp;<em>Entry Level</em>&nbsp;SQL-92 adopted as FIPS 127-2.</td>
</tr>
<tr>
<td>1999</td>
<td><a title="SQL:1999" href="https://en.wikipedia.org/wiki/SQL:1999">SQL:1999</a></td>
<td>SQL3</td>
<td>Added regular expression matching,&nbsp;<a title="Hierarchical and recursive queries in SQL" href="https://en.wikipedia.org/wiki/Hierarchical_and_recursive_queries_in_SQL">recursive queries</a>&nbsp;(e.g.&nbsp;<a title="Transitive closure" href="https://en.wikipedia.org/wiki/Transitive_closure">transitive closure</a>),&nbsp;<a title="Database trigger" href="https://en.wikipedia.org/wiki/Database_trigger">triggers</a>, support for procedural and control-of-flow statements, non-scalar types (arrays), and some object-oriented features (e.g.&nbsp;<a title="Structured type" href="https://en.wikipedia.org/wiki/Structured_type">structured types</a>). Support for embedding SQL in Java (<a title="SQL/OLB" href="https://en.wikipedia.org/wiki/SQL/OLB">SQL/OLB</a>) and vice versa (<a title="SQL/JRT" href="https://en.wikipedia.org/wiki/SQL/JRT">SQL/JRT</a>).</td>
</tr>
<tr>
<td>2003</td>
<td><a title="SQL:2003" href="https://en.wikipedia.org/wiki/SQL:2003">SQL:2003</a></td>
<td>&nbsp;</td>
<td>Introduced&nbsp;<a title="XML" href="https://en.wikipedia.org/wiki/XML">XML</a>-related features (<a title="SQL/XML" href="https://en.wikipedia.org/wiki/SQL/XML">SQL/XML</a>),&nbsp;<a title="SQL window function" href="https://en.wikipedia.org/wiki/SQL_window_function">window functions</a>, standardized sequences, and columns with auto-generated values (including identity-columns).</td>
</tr>
<tr>
<td>2006</td>
<td><a title="SQL:2006" href="https://en.wikipedia.org/wiki/SQL:2006">SQL:2006</a></td>
<td>&nbsp;</td>
<td>ISO/IEC 9075-14:2006 defines ways that SQL can be used with XML. It defines ways of importing and storing XML data in an SQL database, manipulating it within the database, and publishing both XML and conventional SQL-data in XML form. In addition, it lets applications integrate queries into their SQL code with&nbsp;<a title="XQuery" href="https://en.wikipedia.org/wiki/XQuery">XQuery</a>, the XML Query Language published by the World Wide Web Consortium (<a class="mw-redirect" title="W3C" href="https://en.wikipedia.org/wiki/W3C">W3C</a>), to concurrently access ordinary SQL-data and XML documents.</td>
</tr>
<tr>
<td>2008</td>
<td><a title="SQL:2008" href="https://en.wikipedia.org/wiki/SQL:2008">SQL:2008</a></td>
<td>&nbsp;</td>
<td>Legalizes ORDER BY outside cursor definitions. Adds INSTEAD OF triggers, TRUNCATE statement,&nbsp;FETCH clause.</td>
</tr>
<tr>
<td>2011</td>
<td><a title="SQL:2011" href="https://en.wikipedia.org/wiki/SQL:2011">SQL:2011</a></td>
<td>&nbsp;</td>
<td>Adds temporal data (PERIOD FOR)&nbsp;(more information at:&nbsp;<a title="Temporal database" href="https://en.wikipedia.org/wiki/Temporal_database#History">Temporal database#History</a>). Enhancements for&nbsp;<a title="SQL window function" href="https://en.wikipedia.org/wiki/SQL_window_function">window functions</a>&nbsp;and FETCH clause.</td>
</tr>
<tr>
<td>2016</td>
<td><a title="SQL:2016" href="https://en.wikipedia.org/wiki/SQL:2016">SQL:2016</a></td>
<td>&nbsp;</td>
<td>Adds row pattern matching, polymorphic table functions,&nbsp;<a title="JSON" href="https://en.wikipedia.org/wiki/JSON">JSON</a>.</td>
</tr>
<tr>
<td>2019</td>
<td>SQL:2019</td>
<td>&nbsp;</td>
<td>Adds Part 15, multidimensional arrays (MDarray type and operators).</td>
</tr>
</tbody>
</table>
<p>Interested parties may purchase SQL standards documents from ISO,&nbsp;IEC or ANSI. A draft of SQL:2008 is freely available as a&nbsp;<a class="mw-redirect" title="ZIP (file format)" href="https://en.wikipedia.org/wiki/ZIP_(file_format)">zip</a>&nbsp;archive.</p>
<p>The SQL standard is divided into ten parts. There are gaps in the numbering due to the withdrawal of outdated parts.</p>
<ul>
<li>ISO/IEC 9075-1:2016 Part 1:&nbsp;<em>Framework</em>&nbsp;(SQL/Framework). It provides logical concepts.</li>
<li>ISO/IEC 9075-2:2016 Part 2:&nbsp;<em>Foundation</em>&nbsp;(SQL/Foundation). It contains the most central elements of the language and consists of both&nbsp;<em>mandatory and optional</em>&nbsp;features.</li>
<li>ISO/IEC 9075-3:2016 Part 3:&nbsp;<em>Call-Level Interface</em>&nbsp;(<a title="SQL/CLI" href="https://en.wikipedia.org/wiki/SQL/CLI">SQL/CLI</a>). It defines interfacing components (structures, procedures, variable bindings) that can be used to execute SQL statements from applications written in Ada, C respectively C++, COBOL, Fortran, MUMPS, Pascal or PL/I. (For Java see part 10.) SQL/CLI is defined in such a way that SQL statements and SQL/CLI procedure calls are treated as separate from the calling application's source code.&nbsp;<a title="Open Database Connectivity" href="https://en.wikipedia.org/wiki/Open_Database_Connectivity">Open Database Connectivity</a>&nbsp;is a well-known superset of SQL/CLI. This part of the standard consists solely of&nbsp;<em>mandatory</em>&nbsp;features.</li>
<li>ISO/IEC 9075-4:2016 Part 4:&nbsp;<em>Persistent stored modules</em>&nbsp;(<a title="SQL/PSM" href="https://en.wikipedia.org/wiki/SQL/PSM">SQL/PSM</a>). It standardizes procedural extensions for SQL, including flow of control, condition handling, statement condition signals and resignals, cursors and local variables, and assignment of expressions to variables and parameters. In addition, SQL/PSM formalizes declaration and maintenance of persistent database language routines (e.g., "stored procedures"). This part of the standard consists solely of&nbsp;<em>optional</em>&nbsp;features.</li>
<li>ISO/IEC 9075-9:2016 Part 9:&nbsp;<em>Management of External Data</em>&nbsp;(<a title="SQL/MED" href="https://en.wikipedia.org/wiki/SQL/MED">SQL/MED</a>). It provides extensions to SQL that define foreign-data wrappers and datalink types to allow SQL to manage external data. External data is data that is accessible to, but not managed by, an SQL-based DBMS. This part of the standard consists solely of&nbsp;<em>optional</em>&nbsp;features.</li>
<li>ISO/IEC 9075-10:2016 Part 10:&nbsp;<em>Object language bindings</em>&nbsp;(<a title="SQL/OLB" href="https://en.wikipedia.org/wiki/SQL/OLB">SQL/OLB</a>). It defines the syntax and semantics of&nbsp;<a title="SQLJ" href="https://en.wikipedia.org/wiki/SQLJ">SQLJ</a>, which is SQL embedded in Java (see also part 3). The standard also describes mechanisms to ensure binary portability of SQLJ applications, and specifies various Java packages and their contained classes. This part of the standard consists solely of&nbsp;<em>optional</em>&nbsp;features. Unlike SQL/OLB&nbsp;<a class="mw-redirect" title="JDBC" href="https://en.wikipedia.org/wiki/JDBC">JDBC</a>&nbsp;defines an&nbsp;<a class="mw-redirect" title="API" href="https://en.wikipedia.org/wiki/API">API</a>&nbsp;and is not part of the SQL standard.</li>
<li>ISO/IEC 9075-11:2016 Part 11:&nbsp;<em>Information and definition schemas</em>&nbsp;(<a title="SQL/Schemata" href="https://en.wikipedia.org/wiki/SQL/Schemata">SQL/Schemata</a>). It defines the Information Schema and Definition Schema, providing a common set of tools to make SQL databases and objects self-describing. These tools include the SQL object identifier, structure and integrity constraints, security and authorization specifications, features and packages of ISO/IEC 9075, support of features provided by SQL-based DBMS implementations, SQL-based DBMS implementation information and sizing items, and the values supported by the DBMS implementations.<sup id="cite_ref-ISO/IEC_9075-11:2008_44-0" class="reference"><a href="https://en.wikipedia.org/wiki/SQL#cite_note-ISO/IEC_9075-11:2008-44">[41]</a></sup>&nbsp;This part of the standard contains both&nbsp;<em>mandatory and optional</em>&nbsp;features.</li>
<li>ISO/IEC 9075-13:2016 Part 13:&nbsp;<em>SQL Routines and types using the Java TM programming language</em>&nbsp;(<a title="SQL/JRT" href="https://en.wikipedia.org/wiki/SQL/JRT">SQL/JRT</a>). It specifies the ability to invoke static Java methods as routines from within SQL applications ('Java-in-the-database'). It also calls for the ability to use Java classes as SQL structured user-defined types. This part of the standard consists solely of&nbsp;<em>optional</em>&nbsp;features.</li>
<li>ISO/IEC 9075-14:2016 Part 14:&nbsp;<em>XML-Related Specifications</em>&nbsp;(<a title="SQL/XML" href="https://en.wikipedia.org/wiki/SQL/XML">SQL/XML</a>). It specifies SQL-based extensions for using XML in conjunction with SQL. The&nbsp;<em>XML</em>&nbsp;data type is introduced, as well as several routines, functions, and XML-to-SQL data type mappings to support manipulation and storage of XML in an SQL database.&nbsp;This part of the standard consists solely of&nbsp;<em>optional</em>&nbsp;features.</li>
<li>ISO/IEC 9075-15:2019 Part 15:&nbsp;<em>Multi-dimensional arrays</em>&nbsp;(SQL/MDA). It specifies a multidimensional array type (MDarray) for SQL, along with operations on MDarrays, MDarray slices, MDarray cells, and related features. This part of the standard consists solely of&nbsp;<em>optional</em>&nbsp;features.</li>
</ul>
<p>ISO/IEC 9075 is complemented by ISO/IEC 13249&nbsp;<em>SQL Multimedia and Application Packages</em>. This closely related but separate standard is developed by the same committee. It defines interfaces and packages based on SQL. The aim is a unified access to typical database applications like text, pictures, data mining or&nbsp;<a class="mw-redirect" title="Georeference" href="https://en.wikipedia.org/wiki/Georeference">spatial data</a>.</p>
<ul>
<li>ISO/IEC 13249-1:2016 Part 1:&nbsp;<em>Framework</em></li>
<li>ISO/IEC 13249-2:2003 Part 2:&nbsp;<em>Full-Text</em></li>
<li>ISO/IEC 13249-3:2016 Part 3:&nbsp;<em>Spatial</em></li>
<li>ISO/IEC 13249-5:2003 Part 5:&nbsp;<em>Still image</em></li>
<li>ISO/IEC 13249-6:2006 Part 6:&nbsp;<em>Data mining</em></li>
<li>ISO/IEC 13249-7:2013 Part 7:&nbsp;<em>History</em></li>
<li>ISO/IEC 13249-8:xxxx Part 8:&nbsp;<em>Metadata Registry Access</em>&nbsp;<a class="external text" href="https://www.iso.org/standard/73181.html" rel="nofollow">MRA</a>&nbsp;(work in progress)</li>
</ul>
<p>ISO/IEC 9075 is also accompanied by a series of Technical Reports, published as ISO/IEC TR 19075 in 8 parts. These Technical Reports explain the justification for and usage of some features of SQL, giving examples where appropriate. The Technical Reports are non-normative; if there is any discrepancy from 9075, the text in 9075 holds. Currently available 19075 Technical Reports are:</p>
<ul>
<li>ISO/IEC TR 19075-1:2011 Part 1: XQuery Regular Expression Support in SQL</li>
<li>ISO/IEC TR 19075-2:2015 Part 2: SQL Support for Time-Related Information</li>
<li>ISO/IEC TR 19075-3:2015 Part 3: SQL Embedded in Programs using the Java<sup>TM</sup>&nbsp;programming language</li>
<li>ISO/IEC TR 19075-4:2015 Part 4: SQL with Routines and types using the Java<sup>TM</sup>&nbsp;programming language</li>
<li>ISO/IEC TR 19075-5:2016 Part 5: Row Pattern Recognition in SQL</li>
<li>ISO/IEC TR 19075-6:2017 Part 6: SQL support for Javascript Object Notation (JSON)</li>
<li>ISO/IEC TR 19075-7:2017 Part 7: Polymorphic table functions in SQL</li>
<li>ISO/IEC TR 19075-8:2019 Part 8: Multi-Dimensional Arrays (SQL/MDA)</li>
</ul>
<h2><span id="Alternatives" class="mw-headline">Alternatives</span></h2>
<p>A distinction should be made between alternatives to SQL as a language, and alternatives to the relational model itself. Below are proposed relational alternatives to the SQL language. See&nbsp;<a title="Navigational database" href="https://en.wikipedia.org/wiki/Navigational_database">navigational database</a>&nbsp;and&nbsp;<a title="NoSQL" href="https://en.wikipedia.org/wiki/NoSQL">NoSQL</a>&nbsp;for alternatives to the relational model.</p>
<ul>
<li><a title=".QL" href="https://en.wikipedia.org/wiki/.QL">.QL</a>: object-oriented Datalog</li>
<li><a class="mw-redirect" title="4th Dimension (Software)" href="https://en.wikipedia.org/wiki/4th_Dimension_(Software)">4D Query Language</a>&nbsp;(4D QL)</li>
<li><a title="Datalog" href="https://en.wikipedia.org/wiki/Datalog">Datalog</a>: critics suggest that&nbsp;<a title="Datalog" href="https://en.wikipedia.org/wiki/Datalog">Datalog</a>&nbsp;has two advantages over SQL: it has cleaner semantics, which facilitates program understanding and maintenance, and it is more expressive, in particular for recursive queries.</li>
<li><a title="HTSQL" href="https://en.wikipedia.org/wiki/HTSQL">HTSQL</a>: URL based query method</li>
<li><a title="IBM Business System 12" href="https://en.wikipedia.org/wiki/IBM_Business_System_12">IBM Business System 12</a>&nbsp;(IBM BS12): one of the first fully relational database management systems, introduced in 1982</li>
<li><a title="ISBL" href="https://en.wikipedia.org/wiki/ISBL">ISBL</a></li>
<li><a class="mw-redirect" title="Java Object Oriented Querying" href="https://en.wikipedia.org/wiki/Java_Object_Oriented_Querying">jOOQ</a>: SQL implemented in Java as an&nbsp;<a title="Domain-specific language" href="https://en.wikipedia.org/wiki/Domain-specific_language">internal domain-specific language</a></li>
<li><a title="Java Persistence Query Language" href="https://en.wikipedia.org/wiki/Java_Persistence_Query_Language">Java Persistence Query Language</a>&nbsp;(JPQL): The query language used by the Java Persistence API and&nbsp;<a class="mw-redirect" title="Hibernate (Java)" href="https://en.wikipedia.org/wiki/Hibernate_(Java)">Hibernate</a>&nbsp;persistence library</li>
<li><a title="JavaScript" href="https://en.wikipedia.org/wiki/JavaScript">JavaScript</a>:&nbsp;<a title="MongoDB" href="https://en.wikipedia.org/wiki/MongoDB">MongoDB</a>&nbsp;implements its query language in a JavaScript API.</li>
<li><a title="Language Integrated Query" href="https://en.wikipedia.org/wiki/Language_Integrated_Query">LINQ</a>: Runs SQL statements written like language constructs to query collections directly from inside&nbsp;<a title=".NET Framework" href="https://en.wikipedia.org/wiki/.NET_Framework">.Net</a>&nbsp;code.</li>
<li><a title="Object Query Language" href="https://en.wikipedia.org/wiki/Object_Query_Language">Object Query Language</a></li>
<li>QBE (<a class="mw-redirect" title="Query By Example" href="https://en.wikipedia.org/wiki/Query_By_Example">Query By Example</a>) created by Mosh&egrave; Zloof, IBM 1977</li>
<li><a title="QUEL query languages" href="https://en.wikipedia.org/wiki/QUEL_query_languages">Quel</a>&nbsp;introduced in 1974 by the U.C. Berkeley Ingres project.</li>
<li><a class="mw-redirect" title="Tutorial D" href="https://en.wikipedia.org/wiki/Tutorial_D">Tutorial D</a></li>
<li><a title="XQuery" href="https://en.wikipedia.org/wiki/XQuery">XQuery</a></li>
</ul>
<h2><span id="Distributed_SQL_processing" class="mw-headline">Distributed SQL processing</span></h2>
<p><a title="DRDA" href="https://en.wikipedia.org/wiki/DRDA">Distributed Relational Database Architecture</a>&nbsp;(DRDA) was designed by a work group within IBM in the period 1988 to 1994. DRDA enables network connected relational databases to cooperate to fulfill SQL requests.</p>
<p>An interactive user or program can issue SQL statements to a local RDB and receive tables of data and status indicators in reply from remote RDBs. SQL statements can also be compiled and stored in remote RDBs as packages and then invoked by package name. This is important for the efficient operation of application programs that issue complex, high-frequency queries. It is especially important when the tables to be accessed are located in remote systems.</p>
<p>The messages, protocols, and structural components of DRDA are defined by the&nbsp;<a title="Distributed Data Management Architecture" href="https://en.wikipedia.org/wiki/Distributed_Data_Management_Architecture">Distributed Data Management Architecture</a>.</p>
<h2><span id="Criticisms" class="mw-headline">Criticisms</span></h2>
<p>Chamberlin's 2012 paper&nbsp;discusses four historical criticisms of SQL:</p>
<h3><span id="Orthogonality_and_completeness" class="mw-headline">Orthogonality and completeness</span></h3>
<p>Early specifications did not support major features, such as primary keys. Result sets could not be named, and sub-queries had not been defined. These were added in 1992.</p>
<h3><span id="NULLs" class="mw-headline">NULLs</span></h3>
<p>SQL's controversial "NULL" and three-value logic. Predicates evaluated over nulls return the logical value of "unknown" rather than true or false. Features such as outer-join depend on nulls. Null is not equivalent to space. NULLS are not equal to another NULL. NULL represents no data in the column, or row.</p>
<h3><span id="Duplicates" class="mw-headline">Duplicates</span></h3>
<p>Another popular criticism is that it allows duplicate rows, making integration with languages such as&nbsp;<a title="Python (programming language)" href="https://en.wikipedia.org/wiki/Python_(programming_language)">Python</a>, whose data types might make it difficult to accurately represent the data,&nbsp;difficult in terms of parsing and by the absence of modularity.</p>
<p>This can be avoided declaring a unique constraint with one or more fields that identifies uniquely a row in the table. That constraint could also become the primary key of the table.</p>
<h3><span id="Impedance_mismatch" class="mw-headline">Impedance mismatch</span></h3>
<p>In a similar sense to&nbsp;<a title="Object-relational impedance mismatch" href="https://en.wikipedia.org/wiki/Object-relational_impedance_mismatch">Object-relational impedance mismatch</a>, there is a mismatch between the declarative SQL language and the procedural languages that SQL is typically embedded in.</p>

</br>

<h2 id ="Books"> Books</h2>


<ul>

                            
 <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(2).pdf" style="text-decoration:none;">Data Science with Microsoft SQL Server 2016</a></li>

<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(3).pdf" style="text-decoration:none;">Learning SQL</a></li>
 <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(4).pdf" style="text-decoration:none;">Programming Microsoft SQL Server 2012</a></li>                              
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(5).pdf" style="text-decoration:none;">Healthy SQL: A Comprehensive Guide to Healthy SQL Server Performance</a></li>
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(6).pdf" style="text-decoration:none;">Joe Celko's SQL for Smarties</a></li>
 <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(7).pdf" style="text-decoration:none;">Learn SQL Server Administration in a Month of Lunches</a></li>

 <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(8).pdf" style="text-decoration:none;"> Mastering Oracle SQL and SQL*Plus</a></li>
   <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(9).pdf" style="text-decoration:none;">Mastering SQL Queries for SAP Business One</a></li>
  
   
 <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(10).rar" style="text-decoration:none;">Microsoft SQL Server 2012 Bible</a></li>                              
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(11).pdf" style="text-decoration:none;">Practical SQL: A Beginner's Guide to Storytelling with Data</a></li>
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(12).pdf" style="text-decoration:none;">Pro SQL Server on Linux</a></li>
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(13).pdf" style="text-decoration:none;">Real World SQL and PL/SQL</a></li>

<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(14).pdf" style="text-decoration:none;">Sams Teach Yourself Microsoft SQL Server T-SQL in 10 Minutes</a></li>
                              
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(15).pdf" style="text-decoration:none;">Sams Teach Yourself Oracle PL/SQL in 10 Minutes</a></li>

<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(16).pdf" style="text-decoration:none;">SQL For Dummies, 9th Edition</a></li>

  <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(17).rar" style="text-decoration:none;">SQL For Dummies, 8th Edition</a></li>   
  
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(18).pdf" style="text-decoration:none;">SQL in a Nutshell</a></li> 

  
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(19).pdf" style="text-decoration:none;">SQL Primer: An Accelerated Introduction to SQL Basics</a></li> 

<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(20).pdf" style="text-decoration:none;">SQL Server 2017 Integration Services Cookbook</a></li>

<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(21).pdf" style="text-decoration:none;">SQL Server Interview Questions and Answers</a></li>
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(22).pdf" style="text-decoration:none;">Microsoft SQL Server 2012 T-SQL Fundamentals</a></li> 
 <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(23).pdf" style="text-decoration:none;">SQL Stored Procedures and Embedded SQL</a></li> 
 

   <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(24).pdf" style="text-decoration:none;">SQL: Visual QuickStart Guide</a></li>
 
   <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(25).pdf" style="text-decoration:none;">SQL: A Beginner's Guide</a></li>                              
 <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(26).pdf" style="text-decoration:none;">SQL: Easy SQL Programming and Database Management For Beginners. Your Step-By- Step Guide To Learning The SQL Database</a></li>
 <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(27).pdf" style="text-decoration:none;">SQL: with practice exercises, Learn SQL Fast</a></li>
   
 
   <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(28).pdf" style="text-decoration:none;">SQL Injection Attacks and Defense</a></li>
 
   <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(29).pdf" style="text-decoration:none;">SQL: The Complete Reference</a></li>                              

  <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(30).pdf" style="text-decoration:none;">Microsoft course 2778, Writing Queries Using Microsoft SQL Server 2008 Transact-SQL</a></li>
 
   <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(31).pdf" style="text-decoration:none;"> SQL Practice Problems</a></li> 
    <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(32).pdf" style="text-decoration:none;">A guide to the SQL standard</a></li> 

   <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(33).pdf" style="text-decoration:none;">SQL Queries for Mere Mortals</a></li>                              

  <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(34).pdf" style="text-decoration:none;">Oracle PL/SQL Language Pocket Reference</a></li> 
 
  <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(35).pdf" style="text-decoration:none;">Beginning SQL Server Modeling</a></li> 

  <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(36).pdf" style="text-decoration:none;">Pro SQL Database for Windows Azure</a></li> 
 
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(37).pdf" style="text-decoration:none;">PySpark SQL Recipes: With HiveQL, Dataframe and Graphframes</a></li>
 <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(38).pdf" style="text-decoration:none;">Effective SQL</a></li>
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(39).pdf" style="text-decoration:none;">SQL Anywhere Server SQL Reference</a></li>
 <li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(40).rar" style="text-decoration:none;">Microsoft SQL Server 2008 Bible</a></li>                              
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(41).pdf" style="text-decoration:none;">Mastering PostgreSQL 10</a></li>
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(42).pdf" style="text-decoration:none;">Microsoft SQL Server 2005 Analysis Services</a></li>

<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(43).pdf" style="text-decoration:none;">SQL Server 2005 DBA Street Smarts: A Real World Guide to SQL Server 2005 Certification Skills</a></li>
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(44).pdf" style="text-decoration:none;">Microsoft SQL Server 2012 Transact-SQL DML Reference</a></li>
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(45).pdf" style="text-decoration:none;">SQL Server Query Performance Tuning</a></li>

<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(46).rar" style="text-decoration:none;">SQL: Access to SOL Server</a></li>

<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(47).pdf" style="text-decoration:none;">SQL++ For SQL Users: A Tutorial</a></li>
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(48).pdf" style="text-decoration:none;">Tabular Modeling with SQL Server 2016 Analysis Services Cookbook</a></li>
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(49).pdf" style="text-decoration:none;">The Art of SQL</a></li>


<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(50).pdf" style="text-decoration:none;">What's New in SQL Server 2012: Unleash the new features of SQL Server 2012</a></li>
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(51).pdf" style="text-decoration:none;">Advanced Transact SQL for SQL Server 2000</a></li>
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(52).pdf" style="text-decoration:none;">Complete Microsoft SQL Server: Tips and Secrets for Professionals</a></li>

<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(53).pdf" style="text-decoration:none;">SQL Query for SQL Server User's Manual</a></li>
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(54).pdf" style="text-decoration:none;">SQL for MySQL Developers</a></li>
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(55).pdf" style="text-decoration:none;">SQL:
Pocket Guide</a></li>

<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(56).pdf" style="text-decoration:none;">SQL Server Backup and Restore</a></li>
<li><a target="_blank" href="https://github.com/manjunath5496/SQL-Tutorial/blob/master/sql(57).pdf" style="text-decoration:none;">A Developer's Guide to Data Modeling for SQL Server</a></li>



</ul>


