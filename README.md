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
</ul>

</br>


<h2><span id="History" class="mw-headline">History</span></h2>
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



