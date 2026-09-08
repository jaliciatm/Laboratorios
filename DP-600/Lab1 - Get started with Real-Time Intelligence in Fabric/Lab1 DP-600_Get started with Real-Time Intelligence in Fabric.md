**Labotarorio2   DP-600** 

**Get started with Real-Time Intelligence in Microsoft Fabric**

(https://microsoftlearning.github.io/mslearn-fabric/Instructions/Labs/07-real- time-Intelligence.html) 

1. Navigate  to  the[ Microsoft  Fabric  home page ](https://app.fabric.microsoft.com/home?experience=fabric)at https://app.fabric.microsoft.com/home?experience=fabric in  a browser, and sign in with your Fabric credentials. 
1. In the menu bar on the left, select **Workspaces** (the icon looks similar to 🗇). 
1. Create a new workspace with a name of your choice, selecting a licensing mode that includes Fabric capacity (*Trial*, *Premium*, or *Fabric*). 
1. When your new workspace opens, it should be empty. 

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.001.jpeg)

**Create an eventstream** 

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.002.png)

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.003.jpeg)

Select **Next**, then **Connect** to create the eventstream. 

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.004.png)

Select **Open  eventstream**.  The  eventstream  will  show  the **stock** source  and the **stock-data-stream** on the design canvas: 

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.005.jpeg)

**Create an eventhouse** 

The eventstream ingests the real-time stock data, but doesn’t currently do anything with it. Let’s create an eventhouse where we can store the captured data in a table. 

On the menu bar on the left, select **Create**. In the *New* page, under the *Real-Time Intelligence* section, select **Eventhouse**. Give it a unique name of your choice. 

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.006.png)

Select the database, and note that there is an associated *queryset*. This file contains some sample KQL queries that you can use to get started querying the tables in your database. 

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.007.jpeg)

Get data: 

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.008.jpeg)

In the **Select or create a destination table** pane, create a new table named stock. Then in the **Configure the data source** pane, select your workspace and 

the **stock-data** eventstream and name the connection stock-table. 

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.009.jpeg)

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.010.jpeg)

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.011.jpeg)

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.012.jpeg)

The connection between the stream and the table has been created. Let’s verify that in the eventstream. 

In the menu bar on the left, select the **Real-Time** hub. In the **…** menu for the **stock- data-stream** stream, select **Open eventstream**. 

The eventstream now shows a destination for the stream: 

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.013.png)

**Query the captured data** 

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.014.jpeg)

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.015.jpeg)

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.016.jpeg)

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.017.jpeg)

**Create a real-time dashboard** 

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.018.jpeg)

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.019.jpeg)

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.020.png)

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.021.png)

**Clean & Remove** 

![](Aspose.Words.42903e69-e787-4554-a4d8-92ff4748b63e.022.jpeg)
