---
layout: default
title: HOME
---
<div class="alert alert-warning cig">
Are you unable to connect to your Virtual Machine? See this important information for
<a href="https://blogs.technet.microsoft.com/mckittrick/unable-to-rdp-to-virtual-machine-credssp-encryption-oracle-remediation/">how to resolve.</a>
</div>

A charged off loan is a loan that is declared by a creditor (usually a lending institution) that an amount of debt is unlikely to be collected, usually when the loan repayment is severely delinquent by the debtor. Given that high chargeoff has negative impact on lending institutions' year end financials, lending institutions often monitor loan chargeoff risk very closely to prevent loans from getting charged-off.
Using Azure HDInsight ML Server, a lending institution can leverage machine learning predictive analytics to predict the likelihood of loans getting charged off and run a report on the analytics result stored in HDFS and hive tables. 

<div class="alert alert-success">
<h2>Select the platform you wish to explore:</h2>
 <form style="margin-left:30px"> 
    <label class="radio">
      <input type="radio" name="optradio" class="rb" value="cig" >{{ site.cig_text }}, deployed using the 'Deploy to Azure' button on the <a href="START_HERE.html">Quick start</a> page.
    </label>
    <label class="radio">
      <input type="radio" name="optradio" class="rb" value="onp">{{ site.onp_text }}
    </label>
   <label class="radio">
      <input type="radio" name="optradio" class="rb" value="hdi">{{ site.hdi_text }}, deployed using the 'Deploy to Azure' button on the <a href="START_HERE.html">Quick start</a> page.
    </label> 
</form>
</div>
<p></p>
<div class="cig">
On the VM created for you using the 'Deploy to Azure' button on the <a href="START_HERE.html">Quick start</a> page, the SQL Server 2017 database <code>{{ site.db_name}}</code> contains all the data and results of the end-to-end modeling process.  
</div>

<div class="onp">
For customers who prefer an on-premise solution, the implementation with SQL Server ML Services is a great option that takes advantage of the powerful combination of SQL Server and the R language.  A Windows PowerShell script to invoke the SQL scripts that execute the end-to-end modeling process is provided for convenience. <b>Note that you may need to upgrade ML Services to install at least the earliest version that shipped with MicrosoftML package (9.0.1). Instructions to upgrade ML Services on SQL Server 2016 are <a href="https://docs.microsoft.com/en-us/sql/advanced-analytics/r/use-sqlbindr-exe-to-upgrade-an-instance-of-sql-server">here</a></b>.
</div>

<div class="hdi">
This solution shows how to pre-process data (cleaning and feature engineering), train prediction models, and perform scoring on the  HDInsight Spark cluster with Microsoft ML Server deployed using the 'Deploy to Azure' button on the <a href="START_HERE.html">Quick start</a> page.
<p></p>
<strong>HDInsight Spark cluster billing starts once a cluster is created and stops when the cluster is deleted. See <a href="hdinsight.html"> these instructions for important information</a> about deleting a cluster and re-using your files on a new cluster.</strong>

</div>

<p></p>
 We have modeled the steps in the template after a realistic team collaboration on a data science process. Data scientists do the data preparation, model training, and evaluation <span class="sql">from their favorite R IDE.</span><span  class="hdi">using the Open Source Edition of RStudio Server on the cluster edge node.</span>
 <span class="sql">
 DBAs can take care of the deployment using SQL stored procedures with embedded R code.  We show how each of these steps can be executed on a SQL Server client environment such as SQL Server Management Studio.
 </span> 
 <span class="hdi">
 Scoring is implemented with <a href="https://docs.microsoft.com/en-us/machine-learning-server/what-is-operationalization">ML Server Operationalization</a>.
 </span>
 Finally, a Power BI report is used to visualize the deployed results.

<img class="hdi" src="images/hdi.jpg">
<img class="cig" src="images/cig.jpg">
<img class="onp" src="images/onp.jpg">


 


