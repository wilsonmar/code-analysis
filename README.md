# code-management
Currently, all topics are in this one file, which may be split up as this grows.

How can enterprise developers and managers get control of its software assets?

First, an <strong>inventory</strong> is needed.
Metrics include:

 * Number of files in libraries
 * Number of classes, instance methods, interfaces
 * Complexity of code

These can be obtained from <a href="#CodeScanner"> Static Code Scanners to elicit statistics and issues in objects and properties within whole libraries</a>.

But the inventory needs to lead to <a href="#ScopeVisiblity"> visiblity of the scope of work necessary and progress over time</a>. The "work" is to manage code proactively identify:

  * Where memory hogs <a href="#CodeProfiler"> Dynamic profiler of code to analyze memory usage at run-time</a>
  * Where slowness in one module leads to time-outs in modules dependent on them.

For quicker understanding by developers:
  * <a href="#CodeVisualizer"> Visualization of code</a>

  * <a href="#CodeProfiler"> Dynamic profiler of code to analyze memory usage at run-time</a>

<hr />
## <a name="ScopeVisibility"> Scope dashboard</a>
The concept here is like an "accounting system" for the software programming assets over time.
It comes up with counts of various aspects of assets:

  * <strong>Age of code</strong>
  * How much of code is developed by people still around?
  * <strong>What areas in the code is actively worked on</strong>

<a target="_blank" href="https://github.com/acaudwell/Gource/wiki/SVN">
Grouse</a> creates a high-level visualization of a whole repository.


## <a name="CodeScanner"> Static Code Scanners</a>
These automate develop peer reviews.

https://www.wikiwand.com/en/List_of_tools_for_static_code_analysis
lists all of them, including those (like Yasca) which are not actively maintained.

Parasoft is perhaps the most experienced 

 See https://www.youtube.com/watch?v=fLRVcD7EQH8

Parasoft has recently added Service Virtualization with static analysis.

http://www.coverity.com/products/test-advisor-development/

http://www.grammatech.com/codesonar

Many static code analyzers focus on security:
http://www.klocwork.com/products-services/klocwork

Code analysis forensics such as Sextent:
https://www.youtube.com/watch?v=ocmrAOxT0U4

https://www.checkmarx.com/technical-partners/ntobjectives/

Klocwork

<a target="_blank" href="http://www-03.ibm.com/software/products/en/raa">
IBM's Asset Analyzer</a> mines business rules from J2EE code, but uses fossil DB2 COBOL code.

## <a name="CodeVisualizer"> Code Visualizer</a>


## <a name="CodeProfiler"> Dynamic Code Profiler of code to analyze</a>
JProfiler 
