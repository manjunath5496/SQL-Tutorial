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
<div id="toc" class="toc"><br />
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
<li class="toclevel-2 tocsection-12"><span class="toctext"><a href="#Data_control">Data control</a></span></li>
</ul>
</li>
</ul>
</div>



