# Heart-beat

1. User Information: The user is first prompted for their Name, Gender [M/F], and Age in this phase. This data is saved in a text file as soon as the user submits it for the current user. The user's "Medical Report" is created using this data in the final phase.

2. Gather user heart rate data. The user hits the "Start Reading Data" button in this step, which begins reading the data from the "PulseSensor" linked to the Arduino and the laptop over Serial Port. When the button is pressed, two things happen:

a) save_and_plot: In this, the data is collected for upto 3 to 4 minutes and is saved into a CSV file along with Timestamp. Then we pre-process the data using Pandas to provide column names and organize the data in a better way.

b) plotHeartBeat: Once the data collection is complete, this function is called to load the data from the CSV file and a Heart Rate plot is generated for the user and saved as a png file.
