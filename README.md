# code-management
Currently, all topics are in this one file, which may be split up as this grows.

How can enterprise developers and managers get control (show control) of its software assets?

## <a name="Inventory"> Inventory</a>
First, an <strong>inventory</strong> is needed.
Metrics include # of regions, servers, services, executables, files, classes, instance methods, interfaces, lines of code in each.

 * Network nodoes.
 * Regions in the cloud.
 * Servers.
 * Services.
 * Code repositories.

The concept here is like an "accounting system" for the software programming assets over time.
It comes up with counts of various aspects of assets:

  * <strong>Age of code</strong>
  * How much of code is developed by people still around?
  * <strong>What areas in the code is actively worked on</strong>


## <a name="ActionCategories"> Action Categories</a>
The inventory needs to lead to <a href="#ScopeVisiblity"> visiblity of the scope of work necessary and progress over time</a>. The "work" to manage proactively / strategically:

 * <strong>Ignore</strong> what can't go wrong.
 * <strong>Watch</strong> what is going well to keep it that way.
 * <strong>Stabilize</strong> what may be having issues.
 * <strong>Revive</strong> what is exhibiting stress.


## <a name="ScopeVisibility"> Scope dashboard</a>


### <a name="BasisCategories"> Basis for Categories</a>
The basis for determining action category:

  * Had <strong>prior issues</strong>.
  * High percentage <strong>Memory usage</strong> or CPU. 
  * <strong>Slowness</strong> in one module leads to time-outs in modules dependent on them.
  * Spikes in <strong>garbage collection</strong>.
  * Number and importance of <strong>dependencies</strong>.
  * etc.

 
For quicker understanding by developers:
  * <a href="#CodeVisualizer"> Visualization of code</a>
  * Code information can be obtained from <a href="#CodeScanner"> static Code Scanners to elicit statistics and issues in objects and properties within whole libraries</a>.
  * <a href="#CodeProfiler"> Dynamic profiler of code to analyze memory usage at run-time</a>

<hr />

## <a name="CodeScanner"> Static Code Scanners</a>
https://www.wikiwand.com/en/List_of_tools_for_static_code_analysis
lists all of the tools, including those (like Yasca) which are not actively maintained.

These automate develop peer reviews.

<a target="_blank" href="https://github.com/acaudwell/Gource/wiki/SVN">
Grouse</a> creates a high-level visualization of a whole repository.


Parasoft is perhaps the most experienced 

 See https://www.youtube.com/watch?v=fLRVcD7EQH8

Parasoft has recently added Service Virtualization with static analysis.

 * http://www.coverity.com/products/test-advisor-development/

 * http://www.grammatech.com/codesonar

 * https://www.checkmarx.com/technical-partners/ntobjectives/

Many static code analyzers focus on security:

 * http://www.klocwork.com/products-services/klocwork

Code analysis forensics such as Sextent:
https://www.youtube.com/watch?v=ocmrAOxT0U4

<a target="_blank" href="http://www-03.ibm.com/software/products/en/raa">
IBM's Asset Analyzer</a> mines business rules from J2EE code, but uses fossil DB2 COBOL code.

## <a name="CodeVisualizer"> Code Visualizer</a>


## <a name="CodeProfiler"> Dynamic Code Profiler of code to analyze</a>
JProfiler 
