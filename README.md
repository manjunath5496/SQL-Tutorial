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









