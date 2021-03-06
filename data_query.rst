#############
Querying data
#############

.. _sequence_query:

.. index::
   pair: identify; allele sequence

***********************************************
Querying sequences to determine allele identity
***********************************************
Sequence queries are performed in the sequence definition database.   Click 'Sequence query' from the contents page.

.. image:: /images/data_query/sequence_query.png 

Paste your sequence in to the box - there is no need to trim. Normally, you can leave the locus setting on 'All loci' - the software should identify the correct locus based on your sequence.  Sometimes, it may be quicker, however, to select the specific locus or scheme (e.g. MLST) that a locus belongs to. 

.. note::

   If the locus you are querying is a shorter version of another, e.g. an MLST fragment of a gene where the full length gene is also defined, you will need to select the specific locus or the scheme from the dropdown box.  Leaving the selection on 'All loci' will return a match to the longer sequence in preference to the shorter one. 

Click 'Submit'.

.. image:: /images/data_query/sequence_query2.png 

If an exact match is found, this will be indicated along with the start position of the locus within your sequence.

.. image:: /images/data_query/sequence_query3.png 

If only a partial match is found, the most similar allele is identified along with any nucleotide differences. The varying nucleotide positions are numbered both relative to the pasted in sequence and to the reference sequence. The start position of the locus within your sequence is also indicated.

.. image:: /images/data_query/sequence_query4.png 

As an alternative to pasting a sequence in to the box, you can also choose to upload sequences in FASTA format by clicking the file browse button.

.. image:: /images/data_query/sequence_query5.png 

.. index::
   pair: identify; sequence type

Querying whole genome data
==========================
The sequence query is not limited to single genes.  You can also paste or upload whole genomes - these can be in multiple contigs.  If you select a specific scheme from the dropdown box, all loci belonging to that scheme will be checked (although only exact matches are reported for a locus if one of the other loci has an exact match).  If all loci are matched, scheme fields will also be returned if these are defined.  This, for example, enables you to identify the MLST sequence type of a genome in one step.

.. image:: /images/data_query/sequence_query6.png

.. _locus_specific_query:

*****************************************
Searching for specific allele definitions
*****************************************
To retrieve specific allele designations, click 'Sequence attribute search' on a sequence definition database contents page.

.. image:: /images/data_query/sequence_attributes.png

Enter your query using the dropdown search box - additional terms can be added by clicking the '+' button.

Designations can be queried using :ref:`standard operators <query_operators>`.

.. image:: /images/data_query/sequence_attributes2.png

Click submit.

.. image:: /images/data_query/sequence_attributes3.png

Click the hyperlinked results to display allele records.

.. image:: /images/data_query/sequence_attributes4.png

.. image:: /images/data_query/sequence_attributes5.png

Various search criteria can also be selected by combining with filters.  Click the filter heading to display these.

.. image:: /images/data_query/sequence_attributes6.png

Locus-specific attributes
=========================
Some loci have :ref:`extended attribute fields <locus_extended_attributes>`.  To query these, you need to navigate to a locus-specific query page, by clicking the 'locus-specific query' link on the sequence attribute search page.

.. image:: /images/data_query/sequence_attributes7.png

Pick the required locus from the dropdown box.

.. image:: /images/data_query/sequence_attributes8.png

The fields specific for that locus will be added to the dropdown query boxes.

.. image:: /images/data_query/sequence_attributes9.png

.. index::
   pair: browse; scheme profiles

***********************************
Browsing scheme profile definitions
***********************************
If a sequence definition database has schemes defined that include a primary key field, i.e. collections of loci that together create profiles, e.g. for MLST, click the link to 'Browse profiles'. 

.. image:: /images/data_query/browse_profiles.png

Choose the field to order the results by, the number of results per page to display, and click 'Browse all records'.

.. image:: /images/data_query/browse_profiles2.png

Clicking the hyperlink for any profile will display full information about the profile.

.. image:: /images/data_query/browse_profiles3.png

.. index::
   pair: query; scheme profiles

***********************************
Querying scheme profile definitions
***********************************
click the link to 'Search profiles' for the appropriate scheme on the main contents page.

.. image:: /images/data_query/query_profiles.png

Enter the search criteria you wish to search on. You may also see some drop-down list boxes that allow further filtering of results.  You can add search criteria by clicking the '+' button in the 'Locus/scheme fields' section.  These can be combined using 'AND' or 'OR'. 

.. image:: /images/data_query/query_profiles2.png

Each field can be queried using :ref:`standard operators <query_operators>`.

Clicking the hyperlink for any profile will display full information about the profile.

.. image:: /images/data_query/query_profiles3.png

.. _allele_differences:

********************************
Investigating allele differences
********************************

.. index::
   single: sequence similarity; determining

Sequence similarity
===================
To find sequences most similar to a selected allele within a sequence definition database, click 'Sequence similarity' on the contents page.

.. image:: /images/data_query/sequence_similarity.png

Enter the locus and allele identifer of the sequence to investigate and the number of nearest matches you'd like to see, then press submit.

.. image:: /images/data_query/sequence_similarity2.png

A list of nearest alleles will be displayed, along with the percentage identity and number of gaps between the sequences.

.. image:: /images/data_query/sequence_similarity3.png

Click the appropriate 'Compare' button to display a list of nucleotide differences and/or a sequence alignment.

.. image:: /images/data_query/sequence_similarity4.png

Sequence comparison
===================
To directly compare two sequences click 'Sequence comparison' from the contents page of a sequence definition database.

.. image:: /images/data_query/sequence_comparison.png

Enter the locus and two allele identifiers to compare.  Press submit.

.. image:: /images/data_query/sequence_comparison2.png

A list of nucleotide differences and/or an alignment will be displayed.

.. image:: /images/data_query/sequence_comparison3.png

.. seealso::

   :ref:`Locus explorer plugin <locus_explorer>`.

.. _isolate_query:

*********************
Querying isolate data
*********************
The 'Search database' page of an isolate database allows you to search by combinations of provenance criteria, scheme and locus data, and more. 

.. image:: /images/data_query/query_isolates.png

To start with, only one provenance field search box is displayed but more can be added by clicking the '+' button (highlighted). These can be linked together by 'and' or 'or'.

.. image:: /images/data_query/query_isolates2.png

After the search has been submitted, the results will be displayed in a table.

.. image:: /images/data_query/query_isolates3.png

Each field can be queried using :ref:`standard operators <query_operators>`.

More search features are available by clicking the 'Modify form options' tab on the right-hand side of the screen.

.. image:: /images/data_query/query_isolates4.png

A tab will be displayed.  Different options will be available here depending on the database.  Queries will be combined from the values entered in all form sections.  Possible options are:

* Allele designations/scheme field values

  * Search by combination of allele designations and/or scheme fields e.g. ST, clonal complex information.

* Allele designation status

  * Search by whether allele designation status is confirmed or provisional.

* Tagged sequence status

  * Search by whether tagged sequence data is available for a locus.  You can also search by sequence flags.

* Filters

  * Various filters may be available, including

    * Publications
    * Projects
    * MLST profile completion status
    * Clonal complex
    * Sequence bin size
    * Inclusion/exclusion of :ref:`old versions <versioning>` 

.. image:: /images/data_query/query_isolates5.png

If the interface is modified, a button to 'Save options' becomes available within the tab.  If this is clicked, the modified form will be displayed the next time you go to the query page.

.. index::
   pair: allele designations; query
 
Query by allele_designation/scheme field
========================================
Queries can be combined with allele designation/scheme field values.

Make sure that the allele designation/scheme field values fieldset is displayed by selecting it in the 'Modify form options' tab.

.. image:: /images/data_query/query_isolates6.png

Designations can be queried using :ref:`standard operators <query_operators>`.

Additional search terms can be combined using the '+' button.

Add your search terms and click 'Submit'.  Allele designation/scheme field queries will be combined with terms entered in other sections.

.. image:: /images/data_query/query_isolates7.png

.. index::
   single: allele designations; status

Query by allele designation status
==================================
Allele designations can be queried based on their status, i.e. whether they are confirmed or provisional. Queries will be combined from the values entered in all form sections.
 
Make sure that the allele designation staus fieldset is displayed by selecting it in the 'Modify form options' tab.

.. image:: /images/data_query/query_isolates8.png

Select a locus from the dropdown box and either 'provisional' or 'confirmed'.  Additional query fields can be displayed by clicking the '+' button.  Click 'Submit'.

.. image:: /images/data_query/query_isolates9.png

Provisional allele designations are marked within the results tables with a pink background.  Any scheme field designations that depend on the allele in question, e.g. a MLST ST, will also be marked as provisional.

.. index::
   pair: sequence tags; query

Query by tagged sequence status
===============================
Sequence tags identify the region of a contig within an isolate's sequence bin entries that correspond to a particular locus.  The presence or absence of these tags can be queried as can whether or not the sequence has an a flag associated with.  These flags designate specific characteristics of the sequences. Queries will be combined from the values entered in all form sections. 

Make sure that the tagged sequences status fieldset is displayed by selecting it in the 'Modify form options' tab.

.. image:: /images/data_query/query_isolates10.png

Select a specific locus in the dropdown box (or alternatively 'any locus') and a status.  Available status values are:

* untagged

  * The locus has not been tagged within the sequence bin.

* tagged

  * The locus has been tagged within the sequence bin.

* complete

  * The locus sequence is complete.

* incomplete

  * The locus sequence is incomplete - normally because it continues beyond the end of a contig.

* flagged: any

  * The sequence for the  locus has a flag set.

* flagged: none

  * The sequence for the locus does not have a flag set.

* flagged: <specific flag>

  * The sequence for the locus has the specific flag chosen.

.. image:: /images/data_query/query_isolates11.png

.. seealso::

   :ref:`Sequence tag flags <sequence_tag_flags>`

.. index::
   single: filters 

.. _query_filters:

Query filters
=============
There are various filters that can additionally be applied to queries, or the filters can be applied solely on their own so that they filter the entire database.

Make sure that the filters fieldset is displayed by selecting it in the 'Modify form options' tab.

.. image:: /images/data_query/filters.png

The filters displayed will depend on the database and what has been defined within it.  Common filters are:

* Publication - Select one or more publication that has been linked to isolate records.
* Project - Select one or more project that isolates belong to.
* Profile completion - This is commonly displayed for MLST schemes.  Available options are:

  * complete - All loci of the scheme have alleles designated.
  * incomplete - One or more loci have not yet been designated.
  * partial - The scheme is incomplete, but at least one locus has an allele designated.
  * started - At least one locus has an allele designated.  The scheme mat be complete or partial.
  * not started - The scheme has no loci with alleles designated.

.. _seqbin_filter:

* Sequence bin - Specify whether any sequence data has been associated with a record.  Specific threshold values may be selected if these have been :ref:`set up for the database <isolate_xml>`.
* Provenance fields - Dropdown list boxes of values for specific provenance fields may be present if set for the database.  Users can choose to :ref:`add additional filters <modify_query_filters>`.

***************************
Querying by allelic profile
***************************
If a scheme, such as MLST, has been defined for an isolate database it is possible to query the database against complete or partial allelic profiles. Even if no scheme is defined, queries can be made against all loci.  This can also be done in sequence definition databases if the scheme has a primary key field defined.

On the index page, click 'Search by combinations of loci (profiles)' for any defined scheme. Enter either a partial (any combination of loci) or complete profile. 

.. image:: /images/data_query/profile_combinations.png

If multiple schemes are defined, you may have to select the scheme you wish to query in the 'Schemes' dropdown box and click 'Select'.

.. image:: /images/data_query/profile_combinations2.png

Enter the combination of alleles that you want to query for.  Fields can be left blank.

.. image:: /images/data_query/profile_combinations3.png

Alternatively, for scheme profiles, you can enter a primary key value (e.g. ST) and select 'Autofill' to automatically fill in the associated profile.

.. image:: /images/data_query/profile_combinations4.png

Select the number of loci that you'd like to match in the options dropdown box.  Available options are:

* Exact or nearest match
* Exact match only
* x or more matches
* y or more matches
* z or more matches

Where x,y, and z will range from n-1 to 1 where n is the number of loci in the scheme.

.. image:: /images/data_query/profile_combinations5.png

Click 'Submit'.

.. image:: /images/data_query/profile_combinations6.png

***************************************
Retrieving list of isolates or profiles
***************************************
Both isolate and sequence definition databases can be queried against a list of values matching any criteria (isolate provenace fields, alleles, or scheme fields).

Click 'List query' on the main contents page.

.. image:: /images/data_query/list_query.png

Select the attribute you wish to search against in the drop-down list box and enter the list of attributes in the box (one per line).  Click 'Submit'.

.. image:: /images/data_query/list_query2.png

*****************************************
Retrieving isolates by linked publication
*****************************************
Click 'Publications' in the Breakdown section of the contents page.

.. image:: /images/data_query/publications.png

A list of publications linked by isolates within the database will be displayed.

.. image:: /images/data_query/publications2.png

These can be filtered by author and/or year, and the sort order changed.

.. image:: /images/data_query/publications3.png

To display the isolate records for any of the displayed publications, click the  button to the right of the citation.

.. image:: /images/data_query/publications4.png

The abstract of the paper will be displayed (if available), along with all isolates linked to it.

.. image:: /images/data_query/publications5.png

.. index::
   single: options

*************************
User-configurable options
*************************
The BIGSdb user interface is configurable in a number of ways. Choices made are remembered between sessions.  If the database requires you to log on, the options are associated with your user account, whereas if it is a public database, that you haven't logged in to, the options are associated with a browser cookie so they will be remembered if you connect from the same computer (using the same browser).

Most options are set by clicking the 'Set general options' link on the database contents page.  Most of the available options are visible for isolate databases, whereas sequence definition databases have fewer available.

.. image:: /images/data_query/options.png

.. _general_options:

General options
===============
The general options tab is displayed by default.  If another tab is being shown, click the 'General options' header.

.. image:: /images/data_query/options2.png

The general tab allows the following options to be modified: 

* Records per page
* Page bar position
* Nucleotides per line - Some analyses display sequence alignments. This option allows you to set the width of these alignments so suit your display.
* Flanking sequence length - This sets the length of flanking sequence upstream and downstream of a particular locus that is included whenever a sequence is displayed. Flanking sequences are displayed fainter that the locus sequence.
* Locus aliases - Loci can have multiple names (aliases). Setting this option will display all alternative names in results tables.
* Tooltips (beginner's mode) - Most query forms have help available in the form of information tooltips.  These can be switched on/off here.  They can also be toggled off by clicking the Toggle: 'i' button at the top-right of the display of some pages.

Click 'Set options' to remember any changes you make.

.. index::
   pair: options; main results table


Main results table
==================
The 'main results table' tab contains options for the display of paged results
following a query.

Click the 'Main results table' header to display the tab.

.. image:: /images/data_query/options3.png

The 'main results table' tab will scroll up.

.. image:: /images/data_query/options4.png

This tab allows the following options to be modified:

* Hyperlink allele designations - Hyperlinks point to an information page about
  the particular allele definition. Depending on the locus, these may exist on
  a different website.
* Differentiate provisional allele designations - Allele designations can be
  set as confirmed or provisional, usually depending on the method of
  assignment. Selecting this option will display provisional designations in a
  different colour to confirmed designations.
* Information about sequence bin records - Creates a tooltip that displays
  details about sequence tags corresponding to a locus. 
* Sequence bin records - Displays a tooltip linking to the sequence tag if
  available.
* Sequence bin size - Displays the size of the sum of all contigs associated 
  with each isolate record.
* Contig count - Displays the number of contigs associated with each isolate
  record.
* Publications - Displays citations with links to PubMed for each record.

.. index::
   pair: options; isolate record

Isolate record display
======================
The 'isolate record display' tab contains options for the display of a full isolate record.

Click the 'Isolate record display' tab to display the tab.

.. image:: /images/data_query/options5.png

The 'Isolate record display' tab will scroll up.

.. image:: /images/data_query/options6.png

This tab allows the following options to be modified:

* Differentiate provisional allele designations - Allele designations can be set as confirmed or provisional, usually depending on the method of assignment. Selecting this option will display provisional designations in a different colour to confirmed designations.
* Display sender, curator and last updated records - Displays a tooltip containing sender information next to each allele designation.
* Sequence bin information - Displays a tooltip with information about the position of the sequence if tagged within the sequence bin.
* Allele flags - Displays information about whether alleles have flags defined in sequence definition databases.
* Display full information about sample records - Used when the database is used as part of a basic laboratory information management system (LIMS). This option will display records of samples available for the displayed isolate.

.. index::
   pair: options; provenance fields

Provenance field display
========================
The 'provenance field display' tab contains checkboxes for fields to display in the main results table.

Click the 'Provenance field display' tab to display the tab.

.. image:: /images/data_query/options7.png

The 'Provenance field display' tab will scroll up.

.. image:: /images/data_query/options8.png

Some fields will be checked by default - these are defined during :ref:`database setup <isolate_xml_field>` (maindisplay option).

Check any fields that you wish to be displayed and then click 'Set options'.  You can return to the default selection by clicking 'Default' followed by 'Set options'.

.. index::
   pair: options; query

.. _modify_query_filters:

Query filters
=============
The 'query filters' tab contains checkboxes for provenance fields and scheme completion status.  Checking these results in drop-down list box filters appearing in the query page :ref:`filters fieldset <query_filters>`.

Click the 'Query filters' tab to display the tab.

.. image:: /images/data_query/options9.png

The 'Query filters' tab will scroll up.

.. image:: /images/data_query/options10.png

A list of possible filters appears.  Click any checkbox for a filter you would like to make available.  Click 'Set options' when done.  You can return to the default selection by clicking 'Default' followed by 'Set options'.

.. index::
   pair: schemes; modifying display
   pair: loci; modifying display

Modifying locus and scheme display options
==========================================
Whether or not loci, schemes or scheme fields are displayed in result tables, isolate records, or within query dropdown boxes can all be set with default options when first defined.  These attributes can, however, be overridden by a user, and these selections will be remembered between sessions.

The procedure to modify these attributes is the same for locus, schemes or scheme fields, so the steps for loci will be demonstrated only.

Click the appropriate link on the isolate contents page.

.. image:: /images/data_query/locus_options.png

Either select the locus id by querying for it directly.

.. image:: /images/data_query/locus_options2.png

Designations can be queried using :ref:`standard operators <query_operators>`.

Alternatively, you can search by filtering loci by schemes.  Click the 'Filter query by' header and select the scheme in the dropdown box.

.. image:: /images/data_query/locus_options3.png

Once loci have been selected, click Customize 'locus options'.

.. image:: /images/data_query/locus_options4.png

You can then choose to add or remove individual loci from the selection by clicking the appropriate checkboxes.  At the bottom of the page are a number of attributes that you can change - clicking 'Change' will affect all selected loci.

Possible options for loci are:

* isolate_display - Sets how the locus is displayed within an isolate record:

  * allele only - display only identifier
  * sequence - display the full sequence
  * hide - don't show at all

* main_display - Sets whether the locus is displayed in the main results table following a query.

* query_field - Sets whether the locus appears in dropdown list boxes to be used within queries.

* analysis - Sets whether the locus can be used in data analysis functions.

.. note::

   Settings for loci can be overridden by those set for schemes that they are members of.  For example, if you set a locus to be displayed within a main results table, but that locus is a member of a scheme and you set that scheme not to be displayed, then the locus will not be shown.  Conversely, if you set a scheme to be displayed, but set its member locus not to be shown, then that locus will not be displayed (but other loci and scheme fields may be, depending on their independent settings).
