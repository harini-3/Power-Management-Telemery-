Power Management Telemetry Analysis

Project Overview
    The Power Management Telemetry Analysis project focuses on monitoring, analyzing, and comparing CPU usage under various conditions (100%, 70%, 50%, and 30%) on a Windows HP environment. The primary goal is to understand how different CPU usage levels impact system performance by collecting telemetry data. This data includes CPU and memory usage statistics for each application. Insights derived from this data are visualized using Python libraries to provide a clear understanding of performance dynamics under different CPU limitations.

Objective
   - Monitor: Collect detailed telemetry data, including CPU and memory usage for running applications.
   - Analyze: Evaluate the impact of different CPU usage limitations on system performance.
   - Visualize: Display the data through visualizations to enhance understanding and derive insights.

Tools and Packages Used
Tools

   - JupyterLab and Google Colab: Utilized for developing and running Python code for data collection, analysis, and visualization.
   - Windows Task Manager: Employed to observe and monitor real-time system performance.
     
Packages
   - psutil: Used to gather detailed system and process-level telemetry data.
      * Installation: pip install psutil
      * Usage: Retrieving CPU and memory usage, tracking battery status, and monitoring and logging data for each running process.
   - pandas: Facilitates data manipulation and analysis, particularly useful for handling large datasets.
      * Installation: pip install pandas
      * Usage: Organizing data into DataFrames, making it easier to manipulate and prepare data for visualization.
   - matplotlib and seaborn: Primary libraries for creating a variety of visualizations.
      * Installation: pip install matplotlib seaborn
      * Usage: Creating both simple and complex visual graphics, such as bar charts and line plots, to effectively communicate the results of the data analysis.
     
Data Collection
Data was systematically collected to monitor CPU and memory usage under various conditions:

   1. Initial Setup: Configuration of the monitoring system to track and log CPU and memory usage.
   2. Data Recording: Data captured at regular intervals to provide snapshots of system performance across different CPU utilization thresholds.

Steps:

   - Initial Data Collection: Monitoring CPU and memory usage for each running application and recording this data at regular intervals (e.g., every minute) for a specified duration.
      * 100% CPU Usage: Data collected under this condition.
         ![image](https://github.com/user-attachments/assets/a42aaccb-9c31-4b5c-ad85-d90740d4f0ac)
         ![image](https://github.com/user-attachments/assets/d783cf80-abed-4a8d-a079-a81ac696fef9)
         ![image](https://github.com/user-attachments/assets/5cd4bcaf-a09a-428a-9c7c-d5d02c1165b8)
         ![image](https://github.com/user-attachments/assets/85b095d9-4b95-44d1-8169-39084748d1cb)



   - Limiting CPU Usage and Collecting Data: Simulating CPU usage limitations by adjusting process priorities to 70%, 50%, and 30%.
   - collecting the same telemetry data under these conditions.
    
       * 70% CPU Limitation: Data collected under this condition.
         ![image](https://github.com/user-attachments/assets/4333d963-1391-43e4-8e3d-7af12d7bd8cb)
         ![image](https://github.com/user-attachments/assets/53177624-f567-4a2f-bdae-0194847217c1)
         ![image](https://github.com/user-attachments/assets/b81606b2-b0ec-4b18-bc41-e8a70ce5f0c9)
         ![image](https://github.com/user-attachments/assets/49e29192-244a-4439-8ea2-7c9319666af4)

       * 50% CPU Limitation: Data collected under this condition.
         ![image](https://github.com/user-attachments/assets/0f5b9791-d193-4a4a-9847-9f09fe42c680)
         ![image](https://github.com/user-attachments/assets/eae2c4aa-cea5-49ae-8410-877cb9929dad)
         ![image](https://github.com/user-attachments/assets/80b1b9d4-94dc-4c1c-9ddc-2737bd8dfa35)
         ![image](https://github.com/user-attachments/assets/a76d0279-435f-4a82-b1d5-2db3323eaccc)

       * 30% CPU Limitation: Data collected under this condition.
         ![image](https://github.com/user-attachments/assets/4bc6fa54-948c-43da-b8af-e3ef6d6e7f09)
         ![image](https://github.com/user-attachments/assets/99f544d7-0351-4bd1-a565-ef4ae2de969c)
         ![image](https://github.com/user-attachments/assets/2689f323-a41e-4235-9627-8d5f42573b28)
         ![image](https://github.com/user-attachments/assets/fca7fa4c-5a5a-4e91-a863-6388ea8c7eb9)


Data Analysis
The analysis phase involved:
   - Loading and Preparing Data: Data from telemetry collection was loaded into pandas DataFrames.
   - Statistical Analysis: Computation of descriptive statistics such as mean, median, and standard deviation to understand the distribution and variability of CPU usage.
     
     ![image](https://github.com/user-attachments/assets/89e83666-b03d-42fe-bf3d-640ab2269852)

   - Comparative Analysis: Analysis across different CPU usage levels to identify trends and impacts on system performance.
     ![image](https://github.com/user-attachments/assets/05aa33d5-602e-4cbd-b5d0-339004f73757)

Visualization
The visualization phase included:

   - Setup: Configuration of matplotlib and seaborn for generating plots.

   - Graphical Representation: Creation of plots to visually compare CPU usage at different limitation levels, enhancing interpretative clarity of the collected data.
     ![image](https://github.com/user-attachments/assets/1f0d5598-edd6-42b7-ab27-ea51032d54da)

Conclusion
   - This analysis successfully demonstrates the capability to monitor and analyze CPU usage at various simulated levels on a Windows system using a combination of Python tools and techniques. The project highlights how different CPU usage levels affect system performance, providing valuable insights that can guide optimization efforts.
     ![image](https://github.com/user-attachments/assets/9114320b-00d9-4ae7-85cb-b7f8b88f09cf)
   - This report outlines the procedures and findings from the current stage of the project, detailing the methodologies used and the insights gained from the analysis.
   - This project offers a versatile solution for optimizing system performance across Windows, macOS, and Linux platforms. By effectively managing CPU and power usage, it enhances laptop longevity, reduces energy consumption, and ensures smooth operation even under high software demands. The user-friendly design simplifies system monitoring and control, promoting both user satisfaction and environmental sustainability through efficient resource utilization.

