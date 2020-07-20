# Tools for Perfomance Tuning

There are a number of tools and interfaces for performance tuning Cromwell-on-Azure workloads.  These include the following:

### Application Insights

This is a TES-aware set of tools for perf mgmt.  Includes an application map view as well as other views.  Note the nodes which include BLOB storage, CosmosDB, Azure Batch and other services.

![App Map](../images/map.png)

When you drill into the Application Map view, you generated a Filtered Performance View for a particular job run on a particular application now.

![App Map Filtered](../images/app-insights.png)

---

### Azure Batch 

Monitor Azure Batch usage via the WebUI.  This shows resources used by nodes in the virtual cluster.  Node health is also shown here.  

NOTE: Azure Batch Tool (linked) only works with Windows OS.

![Batch](../images/batch.png)

---
### Other Monitoring 
- TES --> CosmosDB job task log query tool (uses SQL API)
    - shows by workflow, `INITIALIZING`, `SYSTEM_FAILURE`, `SUCCESSFUL`, etc...
    - shows configuration for workflows, tasks...
- BLOB store --> use Container Viewer in Azure Portal
    - integrated viewer --> you can upload files ONLY
    - associated viewer --> you can upload/delete folders OR files

