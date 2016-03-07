# reactWise

Wise session to spike out JSON & react rendering for the dashbord overview.
-------------


We could use this in a REST / JSON service for alerts as well as the ocean workflow webapp.

We would transform the data structure built by the DashboardOverviewBuilder to a JSON array of DashboardStatusItem objects.

We would use React JS to render the JSON to the HTML that we current see in the ocean workflow webapp (e.g. http://mainworkflow.prod.gale.web/)


Review the HTML Spike batchedCurrentAndArchive.html.  See how it works, then execute TODO#1 to design JSON 
to represent the dashboard overview, rather than the batch lists.

Once you have the JSON for the dashboard overview, use React JS to render HTML as the workflow webapp.

Here is the HTML you need to render:

```
<table class="dashboard">
		<tbody><tr><th colspan="3">Overview</th></tr>
		
			<tr class="DEFAULT">
			  <td class="DEFAULT-ICON">
			      
			      Running Main Batch Id			  
			  </td>
			  <td>
			        No Main Batch Running
			  </td>
			    <td>
			        
			  </td>
		   </tr>
		
			<tr class="GREEN">
			  <td class="GREEN-ICON">  
			      Last Main Workflow Batch Status 4898-AP			  
			  </td>
			  <td>
			        success
			  </td>
			    <td>
			        Mon Mar 07 15:38:53 EST 2016
			  </td>
		   </tr>
		
			<tr class="GREEN">
			  <td class="GREEN-ICON">			      
			      Last Incremental Workflow Batch Status 4-C on main 4897-CCS			  
			  </td>
			  <td>
			        success
			  </td>
			    <td>
			    
			  </td>
		   </tr>
		
			<tr class="GREEN">
			  <td class="GREEN-ICON">
			      Server Status			  
			  </td>
			  <td>
			        All 109 servers responded
			  </td>
			    <td>
			        Mon Mar 07 15:50:32 EST 2016
			  </td>
		   </tr>
		
			<tr class="YELLOW">
			  <td class="YELLOW-ICON">
			        <span class="dashboard_js">
			          <div style="display: none;"><h2>In Blackout: BlackOutWindowPreCondition</h2><p>We are in the blackout for starting on a new batch</p><p>This condition should correct itself</p></div>
				      <img src="images/Actions-help-about-icon.png" alt="<h2>In Blackout: BlackOutWindowPreCondition</h2><p>We are in the blackout for starting on a new batch</p><p>This condition should correct itself</p>" title="<h2>In Blackout: BlackOutWindowPreCondition</h2><p>We are in the blackout for starting on a new batch</p><p>This condition should correct itself</p>">
				    </span>
			      
			      In Blackout			  
			  </td>
			  <td>
			        Blackout detected due to BlackOutWindowPreCondition
			  </td>
			    <td>
			        Mon Mar 07 15:46:48 EST 2016
			  </td>
		   </tr>
		
			<tr class="DEFAULT">
			  <td class="DEFAULT-ICON">
			      
			      Poller			  
			  </td>
			  <td>
			        Active
			  </td>
			    <td>
			        Mon Mar 07 15:50:33 EST 2016
			  </td>
		   </tr>
		
			<tr class="DEFAULT">
			  <td class="DEFAULT-ICON">
			      AutoRestart			  
			  </td>
			  <td>
			        Active
			  </td>
			    <td>
			        Mon Mar 07 15:50:33 EST 2016
			  </td>
		   </tr>
		
	</tbody></table>
	```