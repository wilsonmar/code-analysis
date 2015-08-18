# code-management
Currently, all topics are in this one file, which may be split up as this grows.

How can enterprise developers and managers get control (show control) of its software assets?

## <a name="Inventory"> Inventory</a>
First, an <strong>inventory</strong> is needed.
Metrics include # of 

 * Network nodoes.
 * Regions in the cloud.
 * Servers.
 * Services.
 * Code repositories
 * executables, files, classes, instance methods, interfaces, lines of code in each.
 * threads

The concept here is like an "accounting system" for the software programming assets over time.
It comes up with counts of various aspects of assets:

  * <strong>Age of code</strong>
  * How much of code is developed by people still around?
  * <strong>What areas in the code is actively worked on</strong>
  * How long to provision a server.
  * Hong long from start to useable
  * Distribution among nodes
  * Lines of code


## <a name="ActionCategories"> Action Categories</a>
The inventory needs to lead to <a href="#ScopeVisiblity"> visiblity of the scope of work necessary and progress over time</a>. The "work" to manage proactively / strategically:

 * <strong>Ignore</strong> what can't go wrong.
 * <strong>Watch</strong> what is going well to keep it that way (depend on automatic alerts for more action)
 * <strong>Stabilize</strong> what may be having issues (investigate possible bottlenecks using extended metrics).
 * <strong>Revive</strong> what is exhibiting stress using a full arsenal of profiler tools, etc.


## <a name="ScopeVisibility"> Scope dashboard</a>


### <a name="BasisCategories"> Basis for Categories</a>
The basis for determining action category:

  * Had <strong>prior issues</strong>, especially customer impact.
  * High percentage <strong>Memory usage</strong> or CPU.
  * Low utilization (over provisioned).
  * Spikes in <strong>garbage collection</strong>.
  * <strong>Slowness</strong> in one module leads to time-outs in modules dependent on them.
  * Number and importance of <strong>dependencies</strong>.
  * Fall-back being available.
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


Parasoft is perhaps the most experienced at applying coding rules:
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
IBM's Asset Analyzer</a> mines business rules from J2EE code, but uses fossil DB2.


## <a name="CodeVisualizer"> Code Visualizer</a>

 * <a target="_blank" href="https://github.com/acaudwell/Gource/wiki/SVN">
   Grouse</a> creates a high-level visualization of a whole repository.

 * http://www.altova.com/umodel/uml-reverse-engineering.html
   generates UML sequence diagrams from models built from scanning code, so
   interactions among classes can be visualized using a modeling program such as 
   Enterprise Architect at http://www.sparxsystems.com/ 


## <a name="CodeProfiler"> Dynamic Code Profiler of code to analyze</a>
A list of code profiler tools is at
https://blog.idrsolutions.com/2014/06/java-performance-tuning-tools/

JProfiler 
