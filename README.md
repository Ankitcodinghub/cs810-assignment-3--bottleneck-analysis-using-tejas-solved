# cs810-assignment-3--bottleneck-analysis-using-tejas-solved
**TO GET THIS SOLUTION VISIT:** [CS810 Assignment 3- Bottleneck analysis using Tejas Solved](https://www.ankitcodinghub.com/product/cs810-assignment3-bottleneck-analysis-using-tejas-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;117995&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS810 Assignment 3- Bottleneck analysis using Tejas Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
            5/5 - (2 votes)    </div>
    </div>
Part A

Get source code of the Tejas architectural simulator from here.

How to set up Tejas:

● Configuration file set-up:

Start with the configuration file (config_tigerLake.xml) and NOC configuration file (NocConfig.txt) given in the folder tejas_resources in the CS810_resources repository.

Make copies of these files and modify them as required.

○ Set EmulatorType to none

○ Set CommunicationType to file

○ Set StoreExecutionTraceInAFile to false

○ Set subsetSimSize to the number of instructions that you want to simulate

○ Set ToCompute (under Criticality) to false

○ Set ReadingFromLeanTrace to false

○ Set NocConfigFile to the full path to the NocConfig.txt file

● Run ant make-jar in the root folder (the folder that contains the file build.xml).

This will create the file tejas.jar in the folder jars/.

● To run Tejas, run java -jar &lt;path-to-jar-file&gt; &lt;path-to-config-file&gt; &lt;path-to-stat-file-to-be-created&gt; &lt;path-to-trace-file&gt;

○ Trace files are available in the folder CPU2017_benchmarks/tejas_traces/ in the CS810_resources repository.

○ Example: java -jar /xyz/tejas.jar /xyz/config_tigerLake.xml /xyz/gcc.stat /xyz/gcc

○ This command simulates the execution of (a portion) of the gcc benchmark on a processor that is described in config_tigerLake.xml and records the statistics in the file gcc.stat .

○ The above example command assumes that tejas.jar, config_tigerLake.xml, gcc_0.gz, and gcc_1.gz are found in the folder

/xyz/.

○ Note that in the command, we should not write _0.gz or _1.gz while mentioning the trace file.

Part B

Play around with the configuration file and identify the “bottleneck” for each SPEC CPU2017 benchmark application. That is, attempt to identify which components of the architecture play the greatest role in determining the application’s performance. Feel free to explore even unrealistic scenarios like perfect caches and perfect branch predictors to help you in your investigation.

Your report must include detailed analysis of each benchmark, with supporting plots as evidence for your claims.
